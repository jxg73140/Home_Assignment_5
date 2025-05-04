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

---

## 🎮 How Does the Adversarial Process Work?

Think of it like a game between a **counterfeit artist** and a **detective**:

- The **Generator** is the artist:  
  - Creates fake data and tries to fool the discriminator.

- The **Discriminator** is the detective:  
  - Looks at data and decides if it’s real or fake.

They are trained **together**:
- Discriminator learns to spot fake data better.
- Generator learns to make more realistic fakes.

> Over time, both improve through competition.

Eventually, the **generator gets so good**, the **discriminator can’t tell fake from real**.

---

## 🎯 Goals of Each Part

| Component      | Goal                                        |
|----------------|---------------------------------------------|
| Generator (G)  | Fool the discriminator with fake data       |
| Discriminator (D) | Tell apart real data from fake data        |

---

## ✅ Summary

- GANs are powerful tools for generating fake-but-real-looking data.
- They work by training two models (G and D) to compete and improve.
- This "game" helps both models get better over time.

---

