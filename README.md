# PyTorch Learning Journey 

A hands-on repository for learning **PyTorch** from the fundamentals to computer vision and deep learning.

The goal of this repository is not just to memorize PyTorch syntax, but to understand **how neural networks work and how to build, train, evaluate, and improve them in practice**.

##  Goals

- Learn PyTorch fundamentals
- Understand tensors and automatic differentiation
- Build neural networks from scratch
- Understand training and validation
- Learn how backpropagation works in practice
- Build and train CNNs
- Learn computer vision with PyTorch
- Experiment with different architectures and hyperparameters
- Eventually apply PyTorch to medical imaging
- Prepare for Kaggle competitions and future thesis work

##  Tools

- Python
- PyTorch
- NumPy
- Matplotlib
- Jupyter Notebook
- Kaggle Notebooks
- Git & GitHub


##  Development Environment

Most experiments can be run locally for learning and debugging.

For larger models and datasets, **Kaggle Notebooks** or **Google Colab** can be used to take advantage of GPU acceleration.

The goal is to keep the code portable between local CPU execution and GPU environments.

Example:

```python
import torch

device = torch.device(
    "cuda" if torch.cuda.is_available() else "cpu"
)

print(device)
```

Models and tensors can then be moved to the appropriate device:

```python
model = model.to(device)
X = X.to(device)
y = y.to(device)
```

##  Learning Philosophy

This repository focuses on **understanding rather than copying code**.

For every major concept, I want to understand:

1. What does it do?
2. Why do we need it?
3. What is happening mathematically?
4. How does PyTorch implement it?
5. What happens if I change it?
6. How does it affect model performance?

Instead of simply following tutorials, experiments will be used to test and reinforce the concepts.



##  Long-Term Goal

The long-term goal is to progress from basic PyTorch exercises to real-world deep learning projects, particularly **computer vision and medical imaging**.

Eventually, the knowledge gained here will be applied to larger projects and Kaggle competitions such as the **RSNA Knee Abnormality Detection** competition.

---

> Learning PyTorch by building, experimenting, breaking things, and figuring out why they broke.
