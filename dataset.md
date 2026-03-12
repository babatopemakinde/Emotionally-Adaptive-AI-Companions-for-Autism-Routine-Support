# Autistic Children Emotions Dataset

## Overview

The **Autistic Children Emotions Dataset** is a facial expression dataset designed to support research in **emotion recognition for autistic children**. It contains facial images categorized into multiple emotional classes and is intended for use in **affective computing, assistive AI systems, and emotion-aware technologies**.

The dataset enables researchers and developers to build models capable of recognizing emotional expressions in autistic adolescents and children. Such systems can contribute to:

- Emotion-aware AI companions  
- Assistive technologies for autism support  
- Behavioral analysis tools  
- Human–computer interaction research  
- Emotion recognition deep learning models  

The dataset was created by **Dr. Fatma M. Talaat** and is publicly available for research and experimentation. :contentReference[oaicite:0]{index=0}

---

## Dataset Download

You can download the dataset from Kaggle:

🔗 **Dataset Link**  
https://www.kaggle.com/datasets/fatmamtalaat/autistic-children-emotions-dr-fatma-m-talaat

This dataset is hosted on Kaggle to support open research in **emotion recognition and autism-related assistive technologies**. :contentReference[oaicite:1]{index=1}

---

## Dataset Structure

The dataset follows a **standard deep learning folder structure**, making it easy to use with frameworks such as **PyTorch, TensorFlow, and Keras**.
Autistic Children Emotions/
│
├── Train/
│ ├── anger/
│ ├── fear/
│ ├── joy/
│ ├── sadness/
│ ├── surprise/
│ └── natural/
│
└── Test/
├── anger/
├── fear/
├── joy/
├── sadness/
├── surprise/
└── natural/


Each folder contains facial images corresponding to a specific emotional category.

---

## Emotion Classes

The dataset contains **six primary emotion categories**:

| Emotion | Description |
|--------|-------------|
| **Joy** | Expressions representing happiness or excitement |
| **Sadness** | Expressions showing sadness or distress |
| **Anger** | Facial expressions indicating frustration or anger |
| **Fear** | Expressions related to fear or anxiety |
| **Surprise** | Expressions showing astonishment |
| **Natural** | Neutral facial expressions |

These categories allow models to learn diverse emotional patterns expressed by autistic children. :contentReference[oaicite:2]{index=2}

---

## Data Format

- **Image Format:** JPG  
- **Color Space:** RGB  
- **Dataset Type:** Supervised classification  
- **Structure:** Class-separated directories  

Example loading using **PyTorch**:

```python
from torchvision.datasets import ImageFolder
from torchvision import transforms

dataset = ImageFolder(
    root="Train",
    transform=transforms.ToTensor()
)


Each folder contains facial images corresponding to a specific emotional category.

---

## Emotion Classes

The dataset contains **six primary emotion categories**:

| Emotion | Description |
|--------|-------------|
| **Joy** | Expressions representing happiness or excitement |
| **Sadness** | Expressions showing sadness or distress |
| **Anger** | Facial expressions indicating frustration or anger |
| **Fear** | Expressions related to fear or anxiety |
| **Surprise** | Expressions showing astonishment |
| **Natural** | Neutral facial expressions |

These categories allow models to learn diverse emotional patterns expressed by autistic children. :contentReference[oaicite:2]{index=2}

---

## Data Format

- **Image Format:** JPG  
- **Color Space:** RGB  
- **Dataset Type:** Supervised classification  
- **Structure:** Class-separated directories  

Example loading using **PyTorch**:

```python
from torchvision.datasets import ImageFolder
from torchvision import transforms

dataset = ImageFolder(
    root="Train",
    transform=transforms.ToTensor()
)

Fatma M. Talaat.
Autistic Children Emotions Dataset.
Kaggle Dataset.
