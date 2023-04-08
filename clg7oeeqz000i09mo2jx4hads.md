---
title: "Yan Lecun and the JEPA of AI"
datePublished: Sat Apr 08 2023 07:50:09 GMT+0000 (Coordinated Universal Time)
cuid: clg7oeeqz000i09mo2jx4hads
slug: yan-lecun-and-the-jepa-of-ai
cover: https://cdn.hashnode.com/res/hashnode/image/stock/unsplash/2Ts5HnA67k8/upload/396f3b6cfa0c0f83f490f949fe68eb0d.jpeg
tags: machine-learning, future, generative-ai, future-of-ai, cognition

---

With some of the points Mr. LeСun rises in [his recent paper](https://readwise.io/reader/document_raw_content/42878391) on generative AI and a proposed architecture called JEPA (Joint Embedding and Prediction Architecture, sounds especially good in Russian).

Let's try to uncover the main points!

# ML and HL

![](https://i.imgur.com/ljaeM4u.png align="left")

Hygh life is not a novelty. Okay, that's actually human learning in comparison to machine learning. Mr. LeCun's quotes are *in italics*.

## Machine learning virgin

### **Supervised learning** (SL)

*Requires large numbers of labeled samples.*

### **Reinforcement learning** (RL)

*Requires insane amounts of trials.*

### **Self-Supervised Learning** (SSL)

*Requires large numbers of unlabeled samples.*

![SSL by LeCun](https://lilianweng.github.io/lil-log/assets/images/self-sup-lecun.png align="left")

SSL by LeCun

![](https://amitness.com/images/self-supervised-workflow.png align="left")

## Human learning Chad

![](https://i.imgur.com/nbQIdK6.png align="left")

In comparison, **human and (not every) animal learning** is much more efficient:

### Causality

* *Understanding how the world works;*
    
* *Can predict the consequences of their actions;*
    

### Reasoning and planning

* *Can perform chains of reasoning with an unlimited number of steps;*
    
* *Can plan complex tasks by decomposing it into sequences of subtasks.*
    

## Auto-regressive LLMs are

likely not the solution. It's a black box approach with correct answer probability of

$$P(correct) = (1-e)^n$$

This diverges exponentially. Of course, there are [some projects](https://arxiv.org/abs/2303.17651) tackling that - but IMO some kind of a stopper, as [with plain generative AI](https://yawn.hashnode.dev/brandolinis-ai-and-an-unexpected-virtue-of-a-research-proposal), is needed.

Think of it as a negative feedback mechanism, an autoreceptor:

![](https://th.bing.com/th/id/R.09f74ef4cd8035931056908a9baf21db?rik=ffH2NsIZcLYU2Q&riu=http%3a%2f%2fschoolbag.info%2fbiology%2fmcat%2fmcat.files%2fimage053.jpg&ehk=LLxqlcpH9nDzAW%2fY5nwyjf2HHI%2fLLK6I2mZb1L1vTbM%3d&risl=&pid=ImgRaw&r=0 align="left")

So, in short words, there are a lot of things going potentially wrong - basically, exponential bullshit risks on any level of effects.

# New kids on the block

## Modular autonomous AI architecture

![](https://i.imgur.com/sHLDQfL.png align="left")

Basically, a [bayesian predicting](https://en.wikipedia.org/wiki/Bayesian_approaches_to_brain_function) regret-minimizing machine. Yeah, it resembles the things Anil Seth mentioned in his "Being You" and [paper](http://sro.sussex.ac.uk/id/eprint/55767/1/The_Cybernetic_Bayesian_Brain.pdf).

Yeah, our brains may really be [Bayesian prediction machines](https://paminy.com/book-summary-being-you-anil-seth-new-science-consciousness/#brains) as per [free energy minimization principle](https://en.wikipedia.org/wiki/Free_energy_principle).

And yeah, regret ~= prediction error here: it's *abs(expectation - reality)*.

P.S. Andrew Gallimore's "Reality Switch Technologies" provides [roughly the same account](https://readwise.io/reader/shared/01gx4939hjb7mtt5074b0zk1j2): prediction errors flow upwards the cognitive hierarchy, and **only mismatch signals are used to update the model (as this delta is what can help minimize the prediction error).**

It consists of:

### Configurator

Basic configuration and update module.

### Perception

The "sensory" part that receives signals.

### World model

One of the main modules: it predicts the future world state.

For that, it should account for world being not fully predictable - a bane of generative models in part causing hallucinations. Yeah, yeah, [contextual and chain prompting](https://cobusgreyling.medium.com/preventing-llm-hallucination-with-contextual-prompt-engineering-an-example-from-openai-7e7d58736162), lots of [practical steps](https://newsletter.victordibia.com/p/practical-steps-to-reduce-hallucination), yada yada yada - still, those are band aids.

![](https://i.imgur.com/K6dbEh7.png align="left")

## Welcome to JEPA

![](https://i.imgur.com/CUzKrlG.png align="left")

* It predicts only an **abstract representation** of *future state, y*
    
* It actively looks for [minimizing the "energy"](https://en.wikipedia.org/wiki/Energy_based_model) by giving higher scoring/priority to incompatible present -&gt; future pairs (x -&gt; y)
    

![](https://i.imgur.com/E6OZzec.png align="left")

### EBMs

A mega-short primer on **Energy-based models**, quoting Wiki: EBMs capture dependencies by associating an unnormalized probability scalar (*energy*) to each configuration of the combination of observed and latent variables. Inference consists of finding (values of) latent variables that minimize the energy given a set of (values of) the observed variables.

**Scalar**: almost a vector, but not:

![](https://www.grc.nasa.gov/www/k-12/airplane/Images/vectors.gif align="left")

**Unnormalized** means the scalars can have a sum of &gt;1, despite what we're used to with probability - a probability space can damn well have it at 146%!

So, in simpler words:

* we have some variants of future *y*, each with a probability of it happening;
    
* we're looking for the value of *y* that is the most probable -&gt; coursing to the next reality node that **everything is converging to.** As Wiki says, this is an advantage: *An EBM can generate sharp, diverse samples or (more quickly) coarse, less diverse samples. Given infinite time, this procedure produces true samples.*
    

![It's Apple's patent net, but still looking like a solid ohmygod-complex-graph I was looking for...](https://miro.medium.com/v2/resize:fit:4800/format:webp/1*UlfG6Q33A88oLXWc4h0BKQ.jpeg align="left")

It's Apple's patent net, but still looking like a solid ohmygod-complex-graph I was looking for...

### Critic/cost module

Assesses and tries to **minimize**:

* information content of *z*, latent configurator variable/vector
    

* the "cost" of traversing to next prediction state, i.e. prediction error (may be wrong here)
    

While **maximizing the information content of present and future states** (akin to [Integrative Information Theory's](https://fully-human.org/what-is-the-integrated-information-theory/) maximality measure)

![](https://i.imgur.com/abXWXzq.png align="left")

### Actor

It acts, huh.

### Short-term memory

Stores state-cost pairs/"episodes".

## Abstractness

Again, YL notes that **low-level representations** (up to the last detail) are **mostly suitable for short-term predictions**. A good example of this is a weather forecast - when trying to predict the next state down to the degree/number of rain drops, we're destined to suffer from a higher prediction error (and soaked documents, yeah).

In contrast, **higher-level**/more abstract (ermmm we're moving towards future, yeah, definitely) are **more "robust"** so to say.

![](https://th.bing.com/th/id/R.dddc4bb17cae1ca22899a9e5d14b5af2?rik=7zHQBBVFCDoSQA&pid=ImgRaw&r=0 align="left")

## Hierarchical planning

Now the important things

* **An action at level *k* specifies an objective for level *k-1*** -&gt;so we're using actions arising from abstract predictions to set lower-level goals. Sounds obvious yet reasonable;
    
* Prediction in higher levels are **more abstract and longer-range.**
    

## Final

### YL proposes

*\* Abandon generative models in favor* ***joint-embedding architectures***

*\* Abandon Auto-Regressive generation*

*\* Abandon probabilistic model in favor of* ***energy-based models***

*\* Abandon contrastive methods in favor of* ***regularized methods***

*\* Abandon Reinforcement Learning in favor of* ***model-predictive control***

*\* Use RL only when planning doesn't yield the predicted outcome, to adjust the world model or the critic.*

### YL defines the following steps

towards Autonomous AI systems:

**Self-Supervised Learning** (*Almost everything is learned through self-supervised learning, and almost nothing - through reinforcement, supervision or imitation*)

* To learn representations of the world
    
* To learn predictive models of the world (*Prediction is the essence of intelligence + common sense*)
    

Handling **uncertainty in predictions**

* [Welcome to JEPA](#)
    
* [EBMs](#)
    

**Learning world models from observation**, like animals and humans: [Human learning Chad](#). Also, emotions/regret/prediction error is quite important: *anticipation of outcomes by the critic or world model+intrinsic cost.*

**Reasoning and planning**: [Hierarchical planning](#)

*Reasoning == simulation/prediction + optimization of objectives* ([Reasoning and planning](#))

* That is compatible with gradient-based learning
    
* No symbols, no logic → vectors & continuous functions
    

## Final words?

*Probabilistic generative models and contrastive methods are doomed.*

![](https://media.tenor.com/I_zDLoRvjkQAAAAC/fifth-element-milla-jovovich.gif align="left")

---

Welcome to **Teleogenic/YAWN/Boi Diaries**❣️

You can find the other blogs I try to cross-post to:

* [**Blog**](https://blog.teleogenic.com)
    
* [**Medium**](https://baldr.medium.com/)
    
* [**Telegram**](https://t.me/ohmyboi)
    
* [**Twitter**](https://twitter.com/ZakharKogan)
    
* Maybe even [**LinkedIn**](https://www.linkedin.com/in/zakhar-kogan/)