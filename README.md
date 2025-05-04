# Student name - Jayadev Goskula (700757314)

## Question 1

A **GAN (Generative Adversarial Network)** is a type of neural network that can create **realistic fake data**, such as:

- Images
- Sounds
- Text

It has **two main parts**:

- **Generator (G)**:  
  - Makes fake data that looks real.

- **Discriminator (D)**:  
  - Tries to tell the difference between real and fake data.

##  How Does the Adversarial Process Work?

Think of it like a game between a **counterfeit artist** and a **detective**:

- The **Generator** is the artist:  
  - Creates fake data and tries to fool the discriminator.

- The **Discriminator** is the detective:  
  - Looks at data and decides if it’s real or fake.

They are trained **together**:
- Discriminator learns to spot fake data better.
- Generator learns to make more realistic fakes.

-Over time, both improve through competition.

Eventually, the **generator gets so good**, the **discriminator can’t tell fake from real**.


## Goals of Each Part

| Component      | Goal                                        |
|----------------|---------------------------------------------|
| Generator (G)  | Fool the discriminator with fake data       |
| Discriminator (D) | Tell apart real data from fake data        |


## Summary

- GANs are powerful tools for generating fake-but-real-looking data.
- They work by training two models (G and D) to compete and improve.
- This "game" helps both models get better over time.

---

## Question 2

##  What Is Misinformation in Generative AI?
Generative AI (like chatbots, image generators, or deepfake tools) can create **content that looks real but is false**. This can lead to the spread of **misinformation** — incorrect or misleading content that people may believe is true.


## Example Application: Fake News Generation
Imagine a generative AI model is used to:
- Create **fake news articles**.
- Generate **realistic images or videos** of public figures saying or doing things they never did.

This can:
- **Confuse people** about what is real.
- **Damage reputations**, especially during elections or crises.
- **Influence public opinion** with false or biased information.

## Harm Mitigation Strategies

### 1. Content Watermarking and Detection
- Add **invisible digital watermarks** or tags to AI-generated content.
- Helps platforms and users **identify AI-generated content** and stop the spread of fake news.

### 2. Fact-Checking and Human Oversight
- Require **human reviewers** to verify important or sensitive content before it is shared widely.
- Use **AI-assisted fact-checkers** to cross-check claims with reliable sources.

## Summary

- Generative AI can create believable fake content, leading to misinformation.
- Harm can be reduced with tools like **watermarking** and **human oversight**.
- Ethical use of AI includes **transparency** and **accountability** in how content is made and shared.

---

## Question 3
Basic GAN Implementation-> This Programming details the implementation of a basic Generative Adversarial Network (GAN) for generating handwritten digits from the MNIST dataset using [PyTorch/TensorFlow]. The project involved designing two neural networks: a Generator, which learns to create realistic-looking fake digits from random noise, and a Discriminator, which learns to distinguish between real MNIST digits and the Generator's fakes.

The training process involved an adversarial loop where the Generator tries to fool the Discriminator, and the Discriminator tries to correctly identify real and fake images. The video showcases the evolution of the generated digits at different training stages: Epoch 0 (initial random noise), Epoch 50 (early, blurry shapes), and Epoch 100 (more defined, though imperfect, digits). Additionally, a plot illustrating the loss trends for both the Generator and Discriminator over the training period is presented to provide insight into the learning dynamics of the GAN.

---

## Question 4
Data Poisoning Simulation-> This Programming simulates a data poisoning attack on a sentiment classifier trained on movie reviews. The aim is to show how manipulating training data can harm model performance, especially regarding "UC Berkeley."

We first trained a basic sentiment classifier [mention type] on a small review dataset. The attack involved finding reviews mentioning "UC Berkeley" and flipping their sentiment labels. The classifier was then retrained with this poisoned data.

We compared the model's accuracy and confusion matrices before and after the attack. The results indicate [describe accuracy change]. The confusion matrices show [explain the specific impact on classifying reviews about "UC Berkeley," e.g., more positive mentions misclassified as negative].

This demonstrates how targeted data poisoning can bias a sentiment classifier's predictions for a specific entity. Even minor data manipulation can significantly affect performance and skew sentiment analysis for the targeted term, highlighting a key security concern in machine learning.

---

## Question 5
# Legal and Ethical Implications of Generative AI

Generative AI models (like GPT) are trained on huge amounts of data from the internet. But this can lead to **legal** and **ethical** problems when:

## 1. Memorizing Private Data

### Example:
- GPT-2 was found to **repeat names, phone numbers, and other private data** from its training set.

### Concern:
- This is a **privacy violation**.
- AI should not remember or share personal information without consent.

## 2. Generating Copyrighted Material

### Example:
- Some AI models can generate content similar to **Harry Potter books** or other copyrighted texts.

### Concern:
- This may **violate copyright laws**.
- Artists and authors may not get credit or payment for their original work.

## Should AI Be Restricted From Certain Data?

### Yes — Here’s Why:
1. **Protects Privacy**  
   - People’s personal data should not be memorized or repeated by AI.

2. **Respects Creators’ Rights**  
   - Writers, artists, and developers deserve credit and control over their work.

3. **Builds Trust**  
   - Ethical AI builds trust with users and avoids legal problems for developers.

## Conclusion

- AI models should be **carefully trained** to avoid using **private or copyrighted data** without permission.
- This helps keep AI **safe, fair, and legal** for everyone.

---

## Question 6
# Aequitas Bias Audit Tool – Equal Parity Metric

## What Is Equal Parity?

**Equal Parity** is a fairness metric that checks if a model gives **positive results** to **different groups at the same rate**.

### Example:
If a model is used to approve loans, Equal Parity asks:
- “Are men and women getting approved at the same rate?”

## Why Is It Important?

- Makes sure **no group is treated unfairly**.
- Ensures **equal opportunity** for everyone.
- Helps detect and reduce **bias and discrimination** in AI systems.

## How Can a Model Fail Equal Parity?
A model fails this test if it gives **more positive results** (like approvals) to one group over another.

### Example:
- **70%** of men are approved.
- Only **30%** of women are approved.
- This shows **bias** — the model fails Equal Parity.

## Summary


**Equal Parity** is a key metric for making sure AI decisions are **fair and inclusive**.






