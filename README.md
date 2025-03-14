# Statistical-Natural-Language-Processing

## Group project: DetectGPT – Zero-shot detection of AI-generated text

This repository contains the implementation of a group project for **COMP0087**: Statistical Natural Language Processing, a course at UCL led by **Dr. Pontus Saito Stenetorp**. Our teaching assistant for the project is **Noah Siegel**.

## 🔍 Project overview

With the rise of LLMs such as ChatGPT, distinguishing between AI-generated and human written text is now a critical challenge.

Here, we implement and analyze **DetectGPT**, a zero-shot detection method introduced by [Mitchell et al. (2023)](https://arxiv.org/abs/2301.11305). The method leverages probability curvature (i.e. the tendency of model generated text to occupy negative curvature regions in the log probability function) to identify synthetic content without requiring any labeled datasets or training a classifier.

## 🚀 Running the code
### 1️⃣ Environment set up
To run DetectGPT on **GPU**, create the following environment and install dependencies:

```sh
conda create --name detect_gpt_gpu python=3.9 -y && \
conda activate detect_gpt_gpu && \
conda install -y numpy pandas tqdm matplotlib && \
conda install -y -c conda-forge transformers sentencepiece && \
conda install -y pytorch torchvision torchaudio -c pytorch -c nvidia && \
conda install -y -c conda-forge sentencepiece
```

### 2️⃣ Running detection
Run the main detection notebook `detectgpt_detection.ipynb`

### 3️⃣ Experimentation
Modify the models, parameters and datasets in the notebook `detectgpt_for_dummies.ipynb` to explore DetectGPT’s performance.

### 📝 Paper Reference
- **Mitchell et al. (2023)**: *DetectGPT: Zero-Shot Machine-Generated Text Detection Using Probability Curvature* ([ArXiv](https://arxiv.org/abs/2301.11305)).
- **Insert paper**

## 📚 Resources & references
- **Project instructions**: [Internet](https://pontus.stenetorp.se/comp0087/)
- **DetectGPT paper**: [ArXiv](https://arxiv.org/abs/2301.11305)
- **Related work**:

## 🤝 Contributors
- Paul Bouyé
- Gianluca Carrozzo
- Hugo Hazard
- Paul Hellegouarch
