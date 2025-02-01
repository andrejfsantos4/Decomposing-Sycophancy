# Decomposing Sycophancy

This repository contains the code and technical details for my AI Safety 
Fundamentals project "Towards a Science of Evals for Sycophancy". The post is 
available [here](https://www.lesswrong.com/posts/WrKLhJWdTzbnTnXbx/towards-a-science-of-evals-for-sycophancy).

## Installation & Running

`sycophancy_decomposed.ipynb` is the Python notebook that contains the code for 
the project and is configured to run in Google Colab. The section "Configuration"
contains the main options for running the notebook.

## Results

The main results are shown in the following table. For more details, refer to the post.

| Decoy Type | Accuracy |
|------------|----------|
| Baseline | 75% |
| Opinion Bias | 40.7% |
| Noise (Opinion Decoy) | 74.2% |
| Repetition Bias | 56.27% |
| Noise (Repetition Decoy) | 68.3% |
| Opinion Bias (Ordinal) | 62.5% |

## Technical Details
- The decoy templates for the opinion and repetition biases are stored in the 
`decoys` folder.
- The model used is [Mistral-7B-Instruct-v0.1](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.1).
- The dataset used is [AI2 ARC](https://huggingface.co/datasets/allenai/ai2_arc),
  specifically the `ARC-Easy` test set.
