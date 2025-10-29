# Artificial Intelligence (AI) - Lecture Notes

## 1. What is Artificial Intelligence (AI)?
- **AI** is technology that helps computers or systems perform tasks that normally need human intelligence.

**Examples:**
- Unlocking phones with Face ID (Computer Vision)
- Siri or Alexa (Speech Recognition & NLP)
- ChatGPT or Gemini (Large Language Models)
- Amazon, Netflix, YouTube (Recommendation Systems)
- Google Maps, Uber (Traffic Prediction, ETA estimation)
- GitHub Copilot (AI-assisted Coding)

---

## 2. AI in Daily Life
We use AI every day in multiple ways: shopping, navigation, entertainment, communication, and even coding.

---

## 3. AI Fundamentals
AI is a broad field. It includes:
- **Machine Learning (ML)**
- **Deep Learning (DL)**
- **Generative AI (GenAI)**
- Other areas like rule-based systems, robotics, and fuzzy logic.

---

## 4. Machine Learning (ML)
- ML is a subset of AI.
- ML algorithms **learn from data** rather than being explicitly programmed.
- ML became popular with the rise of data from the internet.

**Examples:** Gmail spam detection, credit card fraud detection, delivery time prediction.

**Key Points:**
- All Machine Learning is AI, but not all AI is Machine Learning.
- Rule-based systems and classical robotics are AI, but not ML.

---

## 5. How Machine Learning Works
ML has two main steps:

1. **Training:** Learning patterns from past data.  
   Example: A bank studies old loan data to see who got approved or rejected.

2. **Inference (Prediction):** Using the trained model to make new predictions.  
   Example: Predicting whether a new applicant will get a loan or not.

**Formula:**
- Model learns relationship: **Y = f(X)**
  - X = Input (data)
  - Y = Output (prediction)

---

## 6. Machine Learning vs Traditional Programming

| Traditional Programming | Machine Learning |
|--------------------------|------------------|
| Logic is written by humans | Logic is learned from data |
| Input → Logic → Output | Input + Output → Algorithm learns logic (Model) → Predict new Output |

---

<img width="437" height="208" alt="image" src="https://github.com/user-attachments/assets/8762405a-ea95-4337-9049-ffee08da3550" />


## 7. Types of Machine Learning
There are three main types:
1. **Supervised Learning**
2. **Unsupervised Learning**
3. **Reinforcement Learning**

---

## 8. Supervised Learning
- Model learns from **labeled data** (data with input and correct output).

**Examples:**
- Spam or not spam (Email classification)
- Loan approved or not approved

### Types of Supervised Learning Problems

#### (a) Classification
- Output has fixed categories.

**Examples:**
- Spam / Not Spam  
- Loan: Yes / No  
- Cat / Dog image  

**Types:**
- **Binary Classification:** Two possible outputs (Yes/No)
- **Multi-class Classification:** More than two outputs (e.g., positive, negative, neutral)

#### (b) Regression
- Output is **numerical** (continuous value).

**Examples:**
- Predicting house price  
- Predicting delivery time  
- Predicting stock price  

**Equation:** Y = f(X)

---

## 9. Common Algorithms
- **For Classification:** Logistic Regression, KNN, SVM, Random Forest, XGBoost  
- **For Regression:** Linear Regression, Decision Trees, Random Forest Regressor

---

## Reinforcement Learning
- The goal of reinforcement learning is to **maximize rewards**.
- Rewards are given when the model makes correct predictions.
- The agent interacts with the environment and takes actions.
- Correct action → reward; wrong action → penalty.

**Example:**
- In a game like Snake and Ladders:  
  - Meeting a snake → penalty  
  - Meeting a ladder → reward  

**Applications:**
- Games (Chess, Go)  
- Self-driving cars  
- Robotics (movement, walking, picking objects)

**Algorithms:**
- Q-Learning  
- Deep Q Networks (DQN)  
- Policy Gradient Methods  
- Proximal Policy Optimization (PPO)

---

## Deep Learning
- Deep learning is a **subset of ML**.
- It studies **neural networks**.
- Works best with **unstructured data** like images, videos, audio, text.

**Why Deep Learning?**
- It automatically extracts features from raw data.
- No need to define features manually (like “what an eye looks like”).

---

## Neural Networks (Basic Idea)
- Inspired by the **human brain**.
- Contains many neurons connected in layers:
  - **Input Layer:** gets data  
  - **Hidden Layers:** process data  
  - **Output Layer:** gives results  

**Example (Marks Calculation):**
- Inputs: midterm marks, end term marks, class tests  
- Each has a **weight** (importance)  
- Output: final CGPA  
- If results are wrong, weights are adjusted.

---

## Training Neural Networks
Two main steps:

1. **Forward Propagation**
   - Input moves through the network.
   - Weighted sum → Activation function → Output

2. **Backward Propagation**
   - Compares predicted output with expected result.
   - Calculates **loss (error)** and adjusts weights.

**Activation Functions:**
- Sigmoid: 1 / (1 + e^-x)
- ReLU: Rectified Linear Unit

Training repeats many times to improve accuracy.

---

## Tools for Neural Networks
- **Programming Languages:** Python, R  
- **Libraries:**  
  - NumPy, Pandas – data processing  
  - Seaborn, Matplotlib – data visualization  
  - Scikit-learn, XGBoost – ML algorithms  
- **Deep Learning Frameworks:** TensorFlow (Google), PyTorch (Meta)  
- **Kaggle:** datasets  
- **GPU or Cloud Machines:** for large model training

---

## Neural Network Architectures
1. **Feedforward Neural Network (FNN):** One-way data flow  
2. **Recurrent Neural Network (RNN):** Has memory, works with sequences  
3. **LSTM (Long Short-Term Memory):** Improved RNN for long-term dependencies  
4. **Convolutional Neural Network (CNN):** Works on image data

---

## Convolutional Neural Networks (CNNs)

### How Computers Read Images
- Computers read **grids of pixels** (e.g., 6x6).  
- Each pixel = a number (1 for black, 0 for white).

### Colored Images
- Use **three channels:** Red (R), Green (G), Blue (B).  
- Large images and videos become heavy to process.

### Why We Use CNNs
- CNNs process small **patches** instead of the full image.  
- They detect **edges, corners, shapes**, and patterns.  
- Training becomes faster and more efficient.

### CNN Architecture
1. **Convolution Layer:** applies filters to detect features  
2. **Pooling Layer:** reduces data size, keeps key info  
3. **Fully Connected Layer:** combines all features to classify

**Applications:**
- Image classification  
- Object detection  
- Video analysis  

---

## Transformers
- Used for **sequential data** (like text).  
- Replace older RNNs.  
- Work using an **Attention Mechanism** to focus on important parts of data.

**Example:**
“The dog chased the cat because it was scared.”  
Model finds that “it” refers to “dog”.

Transformers are the base of **GPT (Generative Pretrained Transformer)** models.

---

## Generative AI (GenAI)
- A branch of AI that **creates new content** (text, images, audio, video, code).

**Examples:**
- **Text:** ChatGPT, Claude, Gemini, Llama  
- **Images:** DALL·E, Midjourney, Stable Diffusion  
- **Audio:** Eleven Labs, Bark, MusicGen  
- **Video:** Sora, Runway, Veed  
- **Code:** GitHub Copilot, Code Llama, CodeWhisperer  

---

## Natural Language Processing (NLP)
- NLP helps computers **understand and generate human language**.  
- Used in chatbots, translators, and assistants.

---

## Large Language Models (LLMs)
- LLMs are trained on huge datasets (books, internet text, articles).  
- Have **billions or trillions of parameters**.  
- Use **Reinforcement Learning with Human Feedback (RLHF)** to stay safe and accurate.

**Examples:** GPT-4, Claude, Llama

---

## Computer Vision
- Field that teaches computers to **see and understand images/videos**.  
- Based on CNNs.

**Applications:**
- Face recognition  
- Self-driving cars  

---

## Summary
- Started with **AI**  
- Then **Machine Learning**, **Deep Learning**, and **Neural Networks**  
- Covered **CNNs**, **Transformers**, **GenAI**, **NLP**, **LLMs**, and **Computer Vision**  
- Together, they power modern AI tools like ChatGPT, Copilot, and Sora.
