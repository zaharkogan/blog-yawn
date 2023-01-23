# That's MD ChatGPT for you, sir

After ChatGPT [passing the USMLE](https://twitter.com/WatcherGuru/status/1617386607006584832?t=HddOA9sJIYSPgk0NxbZIKw&s=09) I've thought to better test it on some real stuff - medical cases on MedScape.

Say, a [T2D Diabetes patient](https://simulations.medscape.com/edads-121/simulation).

On a side note, here's an [**awesome code-along**](https://www.youtube.com/watch?v=kCc8FmEb1nY) with Andrej Karpathy on making your own GPT:

%[https://www.youtube.com/watch?v=kCc8FmEb1nY] 

# Let's goo

First, a prompt: `You're playing the role of a virtual MD for mock cases. You're knowledgeable, experienced and able to distinguish the real cause of a condition, selecting diagnoses, ordering tests and prescribing medications including their dose and titration regime. I'll send you the patient information in {} and the required information for the next step in [].`

Because yeah, "just an MD" doesn't cut it and generates a wall of rage with the poor GPT not able to sign off diagnoses...

## Tests

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1674457973508/09b904e2-2279-4826-bedb-e69992ad41ea.png align="center")

After supplying the tests results, the following diagnoses were made:

1. `Type 2 Diabetes Mellitus: The patient's HbA1c is elevated at 7.8%, which is above the target range of 4-7%. Additionally, the patient's fasting glucose level is elevated at 156 mg/dL, which is above the normal range of 70-100 mg/dL.`
    
2. `Hypertriglyceridemia: The patient's triglyceride level is elevated at 155 mg/dL, which is above the normal range of 40-150 mg/dL.`
    
3. `Hypercholesterolemia: The patient's total cholesterol level is elevated at 185 mg/dL, which is above the normal range of 0-200 mg/dL.`
    
4. `Low HDL Cholesterol: The patient's HDL cholesterol level is low at 40 mg/dL, which is below the normal range of 40-60 mg/dL.`
    
5. `Obesity: The patient's BMI is 31 kg/m2, which is classified as obesity. It's important to note that, based on the patient's history and physical examination, it may be necessary to consider other potential causes of his symptoms, such as polycystic ovary syndrome (PCOS) or Cushing's syndrome, and order additional tests to rule these out.`
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1674458554173/065a19b4-233b-4d63-a607-692d12a58227.png align="center")

## Medications

`[Continue/Discontinue Current Medications]`  
`[Add medications if needed]`  
`[Add non-medication orders if needed]`

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1674458724479/0ae396b3-1186-4e0c-a34c-4d6c0ea150cc.png align="center")

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1674458809589/dece2b02-cb03-4c92-a152-5a70e83e2254.png align="center")

Now MedScape advises to reconsider adding B12 and liver tests:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1674458892607/549e08a9-c650-42b3-a85e-97bf73892224.png align="center")

Adding in [another AI](https://www.perplexity.ai/?uuid=45f0855e-1606-46f2-81a3-b488e4c32298): *Studies have shown that 10 to 30 percent of patients taking metformin can show signs of reduced vitamin B12 absorption, leading to clinically significant abnormalities* [*<sup>[1]</sup>*](https://www.aafp.org/pubs/afp/issues/2004/0115/p264.html)*. A recent cohort study found that metformin causes vitamin B12 deficiency in 6% of cases* [*<sup>[2]</sup>*](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6867725/#:~:text=It%20has%20been%20reported%20that,deficiency%20due%20to%20metformin%20use.&text=In%20addition%2C%20some%20studies%20have,and%20dose%20of%20metformin%20use.)*. Additionally, a cross-sectional study found that metformin at ≥1500 mg/d could be a major factor related to vitamin B12 deficiency* [*<sup>[2]</sup>*](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6867725/#:~:text=It%20has%20been%20reported%20that,deficiency%20due%20to%20metformin%20use.&text=In%20addition%2C%20some%20studies%20have,and%20dose%20of%20metformin%20use.)

`{You can reconsider adding B12 blood test and Liver Function Tests (LFTs) if needed}`

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1674459064102/e1b63515-eed1-4b01-8515-76389fe31f6a.png align="center")

*So nice for an absolute-attention AI to thank for bringing something to its attention ❣️*

## Results

All in all, ChatGPT seemed to do pretty well considering giving it all the information 🤔

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1674459365576/70ff23a6-4e2e-4894-af9a-761b9d174ac1.png align="center")

## Closing remarks

While networks like ChatGPT can already be good assistants and save a lot of time + note important points, I'm sure they won't replace highly-qualified physicians - at least in the nearest future. <s>After all, a prostate exam requires an examiner ( ͡° ͜ʖ ͡°)</s>