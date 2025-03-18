# Lab Project: Identifying Probability Distributions

This project contains two 1D samples (each of length 1500) and a series of Python scripts/notebooks that analyze them to determine which probability distributions they might follow.

## Project Overview

- **Goal**: Given two data samples (`sample_1.npy` and `sample_2.npy`), we want to:
  1. Plot their histograms with different bin settings to observe the shape.  
  2. Propose a likely distribution (e.g., uniform, exponential, etc.).  
  3. Estimate parameters “by eye” (or via quick numeric checks) so that a theoretical distribution overlays or approximates the empirical data.  
  4. Provide short reasoning for why each distribution seems appropriate.

- **Key Operations**:  
  - Load `.npy` files.  
  - Compute basic statistics (min, max, mean, std).  
  - Plot and compare distributions (overlay PDFs or synthetic samples).  
  - Write a brief explanation of the final chosen distribution and fitted parameters for each sample.

## Files

- **`sample_1.npy` and `sample_2.npy`**: The two data samples (NumPy arrays).  
- **`part1.ipynb` and `part2.ipynb`**: Jupyter/Colab notebooks that:
  - Load the samples.  
  - Demonstrate histogram plotting with various bin settings.  
  - Overlay a theoretical PDF or a synthetic dataset.  
  - Explain the final choice of distribution and parameters.  
- **`README.md`**: (This file) A short description of the project and how to run it.

## How to Run

1. **Open in Google Colab**:  
   - Upload the `.ipynb` notebooks and both `.npy` files to your Colab environment (or place them in the same local folder if you’re using Jupyter locally).
2. **Install any dependencies** (if needed):  
   ```bash
   !pip install numpy matplotlib scipy
   ```

## Interpretation & Results

- **Sample 1**: Flat, uniform‐like data between ~50 and 51. Proposed distribution: `Uniform(50, 51)`.  
- **Sample 2**: Strictly nonnegative, heavily skewed data. Proposed distribution: `Exponential(λ ≈ 1000)`.

In the text cells, you’ll find short justifications for these conclusions (shape, numeric properties, overlay plots).

## Special thanks
Thank you ChatGPT for writing this **`README.md`** for me!
