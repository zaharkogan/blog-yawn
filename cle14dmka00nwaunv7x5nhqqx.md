# Brandolini's AI, and an unexpected virtue of a research proposal

## **Bullshit AImetry principle**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1676126596863/6ce20c5d-9b31-49bf-ae21-8d8a052a4e77.png align="center")

As we've discussed [before](https://hashnode.com/post/cldiez31d01ctxfnvdfb9hb8v), Brandolini's law states that generating unverified information is an order of magnitude easier than refuting it. It seems to climax with generative AI: erroneous facts can cost billions, as in the late case of [Google's Bard advertisement](https://www.npr.org/2023/02/09/1155650909/google-chatbot--error-bard-shares), or just the calculation errors as in Zillow's case with [overvalued home buying](https://insidebigdata.com/2021/12/13/the-500mm-debacle-at-zillow-offers-what-went-wrong-with-the-ai-models/).

In short, checking a model's output requires:

* Knowing the area - you can’t check a proposed microservice architecture if you’re not an architect;
    
* Spending the resources/energy to check;
    
* Being critical - spotting a possible error and re-checking it without the halo effect applicable to the AI ([it’s a kind of magic, magic, MAGIC](https://www.youtube.com/watch?v=4NUSAulJpN8))
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1676126610349/d4c7d067-de7b-460a-a96d-02c6de8bca47.png align="center")

This brings us to, in my opinion, a problem that arises:

## How do we know the truth?

We don't need to know the absolute truth, obviously - it’s individual, in the eye of the beholder, yada yada. But we need to distinguish the factual truth from ‘opinionated’ truth, may I say so. Let’s visit [Wikipedia](https://en.wikipedia.org/wiki/Truth#Coherence) as [Stanford](https://plato.stanford.edu/entries/truth/) doesn’t have the consensus theory.

So, I propose to have a look at [correspondence](https://en.wikipedia.org/wiki/Correspondence_theory_of_truth), [coherence](https://en.wikipedia.org/wiki/Coherence_theory_of_truth), [pragmatic](https://en.wikipedia.org/wiki/Pragmatic_theory_of_truth) and [consensus](https://en.wikipedia.org/wiki/Consensus_theory_of_truth) theories and look at them in a kind of a spectrum (as always, yeah). Yeah, verifying the truth itself, ‘cause why not.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1676126700969/d1bc4454-c4c1-4c32-89da-696acd790368.png align="center")

### Truthing the truth

For us to be OK with the results of, say, a newborn god-AGI, they’ve got to be:

**In accordance with the facts and** [**first principles**](https://en.wikipedia.org/wiki/First_principle) **as per correspondence theory**

You don’t want a flat earth made of gorgonzola.

**(Usually) fitting into the current systems of beliefs/truths as per coherence theory**

I.e. there is a place for contrarian thinking, and discoveries, but not when you’re asking for particular dates or, say, code.

**Usable and useful in practical terms as per the pragmatic theory**

Otherwise, what’s the point in truth if it doesn’t help progress, get happier, eliminate suffering, generate porn fanfics, and revert entropy after all?

**Agreed upon by the feedback as per consensus theory**

It’s a frontier that can be both a blessing and a curse - a potential attack vector for the AI and the community. But agents’ and/or environment agreement and feedback can be crucial. A kind of self-supervised consensus from the unfolding future’s feedback can be modelled, IMO, from the [OODA loop](https://en.wikipedia.org/wiki/OODA_loop). Modified, of course:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1676126717306/fc2a9ca9-6a70-4f4e-9608-a817225bd372.png align="center")

Another assumption - **this all can’t be 100%.** We can only be so much confident in something and have a probability of being correct. So, it’s all going a way of kinda-bayesian updating:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1676126741791/7b6eb4d1-056e-4035-aa2d-4593d69bdced.png align="center")

## How do we model an AI to account for (not only) that?

I’m sure superminds are working on that right now, but let’s imagine I’m sitting in a box (okay, barrel) and speaking with myself:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1676126760875/abd79fc2-38fd-4fc2-b1ed-c745e5cdf3de.png align="center")

Another thing to account for is unfolding circumstances and uncertainty. As we’ve moved from [VUCA to BANI](https://t.me/ohmyboi/916), incomprehensible complexity, and non-linearity are ruling with ambiguousness still in place.

Agents that operate successfully (I won’t delve further here) should:

* find **optimal strategies** to operate under, again, [uncertainty and risk](https://www.toolshero.com/decision-making/decision-making-under-uncertainty): basically, maximize the expected value of actions. It resembles [Sharpe Ratio](https://en.wikipedia.org/wiki/Sharpe_ratio), but in life:
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1676126871480/b0771e98-879a-4604-aa03-3a0112e36e12.png align="center")
    
* be **teleogenic**: [teleogenesis](https://en.wikipedia.org/wiki/Teleogenesis) is, in simple terms, self-setting goals. An even simpler example: you’re buying PB&J to make a sandwich:
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1676126885759/301ac11b-d4a1-4d95-9dcb-6ccbb8b2e659.png align="center")
    
* teleogenesis presumes [**adaptability**](https://en.wikipedia.org/wiki/Adaptability)**:** an adaptable system can change its behaviour (and itself) in response to feedback/conditions;
    
* **understand**, and not just generate. We’ve come closer to understanding [what distinguishes us from an AI at the moment](https://t.me/ohmyboi/1103), and it’s changing the neural representation in time - changing the network itself as it learns more. One of the approaches to start capturing that is, IMO, [causal learning](https://www.course5i.com/blogs/causal-learning-in-ai) - *“capturing the causal mechanism based on the observed data, a new set of variables and assumptions, and incorporate the changes in data distribution when subject to different interventions”*
    
* understanding, closer to first principles the better, helps bring insights and actions that are closer to **factual, coherent and pragmatic truth**
    

For an artificial intelligence system, and I’m talking more integrative stuff, that means being able to:

* [self-tune](https://en.wikipedia.org/wiki/Self-tuning), in the case of ML - that starts with the [AutoAI concept](https://en.wikipedia.org/wiki/AutoAI) and, not the least, [reward functions](https://arxiv.org/abs/2112.08438). A faulty and/or inflexible reward function can [cause a lot of problems](https://openai.com/blog/faulty-reward-functions/), so we need to [learn doing it](https://ai.stackexchange.com/questions/22851/what-are-some-best-practices-when-trying-to-design-a-reward-function)
    
* draw causal relationships and infer from that (please [take a look at chapters](https://ff13.fastforwardlabs.com/) on (3) The great lie of ML, Dangers of spurious correlations, and (6) Causal graphs)
    
* ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1676126908321/243ffdc2-e146-4844-a5e3-ff57fa40d647.png align="center")
    
    prune and change its structure akin to [evolution](https://www.encyclopedia.com/earth-and-environment/ecology-and-environmentalism/environmental-studies/neutrality-theory-evolution) and [neutrality theory](https://t.me/ohmyboi/975), as well as [synaptic pruning](https://en.wikipedia.org/wiki/Synaptic_pruning)
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1676127010191/28bc07d5-891d-45b8-9aed-76b242c06b8b.png align="center")

in the end comes **teleogenesis:** not just choosing the best model, but *setting a task to choose the best model,* i.e. understanding *how to get to some goal*. Here, I presume, we’ll come to an AI alignment and ethic problem - and this may well be the stepping stone most researchers wouldn’t want or just won’t tread onto. However - [if you don’t do something, someone else will](https://vanschneider.com/blog/if-you-dont-do-it-someone-will/), as a bedrock maxim, stands true here IMO

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1676127035660/545f5a4a-25c8-4a32-8051-3637630610bd.png align="center")

## Quantitative limits and qualitative changes

One more crucial thing is resource intensiveness. Evolutionary/simulating algorithms may eventually take a forbiddingly high toll on resources, requiring more and more to (FEED ME) be trained and used for inference. There are some approaches, such as (getting billions of funding ahem cough) using decentralized computation.

Luckily, some other approaches exist.

First, guys from Snorkel proposed an [approach to distilling knowledge from so-called foundational models into a smaller fine-tuned model](https://snorkel.ai/better-not-bigger-how-to-get-gpt-3-quality-at-0-1-the-cost/). Resembles increasing the abstraction levels, doesn't it?

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1676127094364/0cfb6273-0f7b-46f6-acaa-441a24832c67.png align="center")

### Elegantly modelling the Elegans

Another thing that caught my mind recently was a news article on [liquid neural networks](https://www.quantamagazine.org/researchers-discover-a-more-flexible-approach-to-machine-learning-20230207/). The authors propose a somewhat [new approach](https://www.nature.com/articles/s42256-022-00556-7), trying to model the neuronal model and, it seems, succeeding:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1676127107884/4a534674-6d83-4fea-bf77-3561116b68e0.png align="center")

They're claiming both higher accuracy, and lower resource requirements:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1676127117028/519b2347-0e2f-4fb7-a593-c295d27d6850.png align="center")

and (!) achieving high adaptability with a fraction of complexity - say, a liquid network consisting of 19 neurons and 253 synapses [could drive a car](https://www.nature.com/articles/s42256-020-00237-3).

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1676127123839/ecbec620-e999-4dce-93f2-e1323af92637.png align="center")

Their findings on improving current research align well with my ramblings on **pruning** and **connecting** **neurons**:

> The next step, Lechner said, “is to figure out how many, or how few, neurons we need to perform a given task.” The group also wants to devise an optimal way of connecting neurons. **Currently, every neuron links to every other neuron, but that’s not how it works** in *C. elegans*, where **synaptic connections are more selective**. Through further studies of the roundworm’s wiring system, they hope to determine which neurons in their system should be coupled together.

### Distribute every neuron!

Some of the models can be run distributed, e.g. LLMs with [petals package](https://github.com/bigscience-workshop/petals):

![](https://camo.githubusercontent.com/58732a64488a9be928e25f3e60e3692b989ffe212ac86cb4902d8df20a042b03/68747470733a2f2f692e696d6775722e636f6d2f525459463379572e706e67 align="left")

Not a solution, but still a viable first step to edge/hivemind?

> While our platform focuses on BLOOM now, we aim to support more [foundation models](https://arxiv.org/abs/2108.07258) in future.

## Intermediate thoughts

I reckon that AI systems can be viewed as a subset of complex systems, with the propensity of becoming [complex adaptive systems](https://en.wikipedia.org/wiki/Complex_adaptive_system). CAS follow a set of rules, sometimes pretty simple - e.g. GoL and birds flocking behaviour:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1676127134634/f1a5b6a2-8ac1-4276-8c39-f99e6f31ed4a.png align="center")

### Proposal

We can derive from some findings of [mean-field game theory](https://en.wikipedia.org/wiki/Mean-field_game_theory) (it studies small agents in extremely large populations) and [evolutionary game theory](https://en.wikipedia.org/wiki/Evolutionary_game_theory) (self-explanatory) as well as [evolutionary algorithms](https://en.wikipedia.org/wiki/Evolutionary_algorithm), [multi-armed bandits](https://en.wikipedia.org/wiki/Multi-armed_bandit), and in the end, we could come out with <mark>a framework akin to </mark> [<mark>mechanism design</mark>](https://en.wikipedia.org/wiki/Mechanism_design)<mark>-inspired, that will be useful for designing/simulating multi-agent cooperative or competitive behaviour in complex and changing systems for achieving simple, and more complex, goals</mark> (*e.g. anything from an ensemble of trading robots to simulating a voting process, or a marketing simulation as well as factory robots*). I.e. something that will define and guide (AI terms in brackets):

* **population size, its structure, and changing nature** (neurons and layers, changing structure and pruning the ‘unnecessary’ ones + possibly individual 'epochs' for every agent)
    
* optimal **resource allocation** (computational power directed to each neuron, or agent, as per its exploration/exploitation and fitness success; defining sub-populations for sub-goals and allocating resources to those)
    
* **incentives** and subsequent **feedback loops**, positive and negative (reward functions)
    
* **agent interactions**, their **types**, and **parameters** (synapses and neuron connections + activation/inhibition functions)
    
* the **environment in accordance with the final objective, its changing parameters** (the feedback/supervision the agents are receiving + their ability to act semi-autonomously + second-order environment changes from actor actions + environment spontaneous mutation rate ⇢ defining sub-goals to achieve the final goal)
    
* **understand the** [**causal relationships**](https://bdtechtalks.com/2021/03/15/machine-learning-causality/) ([causal](https://las.inf.ethz.ch/6334-2), not correlative-generative, learning)
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1676127140616/778e7dc8-79d2-400e-9f5d-ff6c7b60db1f.png align="center")

I agree that this steers closer and closer to emulating the brain(s) of semi-sentient beings in a cooperative-competitive landscape - or, basically, the world? But let’s try distilling that, tackling the advantages and disadvantages of systems of different natures:

* we shouldn’t repeat the errors found in current biological brains, e.g. self-reinforcing positive loops [such as sugar](https://www.sciencealert.com/research-shows-sugar-can-change-your-brain-here-s-how);
    
* we should, in the case of designing digital systems, take advantage of their nigh-absolute memory and choose the learning rate/everything;
    
* in the case of designing mainly but not only social systems, but we must also avoid possible [agent attack vectors](https://www.csoonline.com/article/3613932/how-data-poisoning-attacks-corrupt-machine-learning-models.html) and, again, [self-reinforcing for objective optimization](https://yawn.hashnode.dev/models-for-the-mental#heading-goodharts-law), i.e. Goodhart’s law;
    
* the approach should be modular, having a set of models for each step/area aforementioned;
    
* preferably, the [simpler/less computationally expensive](https://github.com/powerapi-ng/pyRAPL), the better - if we plan on implementing that in a decentralized way (say, on a decentralized machine like the EVM), that may hold merit;
    
* also, there ideally could/should be ways of achieving approximate solutions with fewer resources, incl. time, spent. I.e. a 70-80% confident result with 20% of resources spent - a [Pareto kind of probing and testing](https://marcusguest.medium.com/chapter-10-an-approach-to-strategy-for-an-uncertain-world-e8c0136797af).
    

---

Welcome to **YAWN/Boi Diaries**❣️ You can find the other blogs I try to cross-post to:

* [**Hashnode**](https://yawn.hashnode.dev/)
    
* [**Medium**](https://baldr.medium.com/)
    
* [**Telegram**](https://t.me/ohmyboi)
    
* [**Twitter**](https://twitter.com/ZakharKogan) (for a lot of stuff)
    
* Maybe even a [**LinkedIn**](https://www.linkedin.com/in/zakhar-kogan/)?