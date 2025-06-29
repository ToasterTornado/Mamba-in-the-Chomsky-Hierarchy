# 🧠 Mamba-SSM in the Chomsky Hierarchy

This repository contains the official code and documentation for my Bachelor Thesis:  
**"Mamba-SSM in the Chomsky Hierarchy: Evaluating Mamba-SSM’s Potential Using Synthetic Tasks"**  

## 📘 Abstract

Sequence modeling gives the foundation for state-of-the-art language models and timeseries forecasting, yet transformers suffer quadratic compute and memory growth with sequence length. Mamba-SSM, a Selective State-Space Model, promises linear-time complexity by dynamically gating its state updates and using a diagonal-plus-low-rank parameterization. In this thesis, we present the first systematic evaluation of Mamba-SSM across fifteen synthetic benchmarks from the first three levels of the Chomsky hierarchy—regular, context-free, and context-sensitive grammars. We train three architectural variants (binary classifier, five-way classifier, generative) at hidden dimensions of 64, 128, and 256, using 4,000 pre-generated batches per epoch over three epochs, and compare against published RNN, xLSTM, and Transformer baselines. Our findings show that Mamba-SSM attains up to 100% accuracy on context-free tasks (Reverse String, Stack Manipulation), struggles near random on regular tasks like Parity Check, and yields good but still mixed results on context-sensitive problems (100% on Bucket Sort but 50% on Missing Duplicate).


## 📂 Repository Structure
- Generate_Data.ipynb: Contains the code to generate the data of the 15 different synthetic tasks
- Data Analysis.ipynb: Contains code snippets to analyze the data and model performances
- utils.py: Contains some useful functions used in the project
- pipeline.ipynb: Contains the entire pipeline with training, evaluation and model-specifications
- Mamba_in_the_Chomsky_Hierarchy.pdf: The written thesis itself
