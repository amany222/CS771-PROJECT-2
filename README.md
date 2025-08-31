# Lifelong Domain Adaptation on CIFAR-10

This project was developed as part of **CS771: Introduction to Machine Learning (Autumn 2024)** under the guidance of **Prof. Purushottam Kar**.  
It explores **lifelong learning and domain adaptation** for image classification on CIFAR-10 datasets using **Learning without Forgetting (LwF)** and **pseudo-labeling**.



## Project Overview
- Implemented **Lifelong Learning** using a **MLP feature extractor** and a **Lightweight Perceptron (LwP) classifier**.  
- Used **pseudo-labeling** for adapting models to unseen datasets without true labels.  
- Addressed the challenge of **catastrophic forgetting** while incrementally training across datasets **D1–D20**.


-

## Methodology
1. **Task 1 (D1–D10)**  
   - Train on labeled dataset D1.  
   - Incrementally update the model with pseudo-labeled data from D2–D10.  
   - Evaluate performance on all datasets after each step.  

2. **Task 2 (D11–D20)**  
   - Extend the model to new domains using pseudo-labeling.  
   - Adapt without access to true labels, leveraging knowledge from previous tasks.  
   - Evaluate across D1–D20 for accuracy retention.  



## Results
- Achieved **~24% accuracy per dataset** in a lifelong learning setup (D1–D10).  
- Mitigated **catastrophic forgetting** with LwF.  
- Demonstrated successful **domain adaptation** via pseudo-labeling across D11–D20.  
- Accuracy matrix shows balanced retention and adaptation over 20 datasets.  






