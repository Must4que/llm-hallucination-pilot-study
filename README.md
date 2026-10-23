# Does Asking an LLM to Answer Only from a Given Text Reduce Hallucinations?

**Author:** MD Mustaque Hossain  
**Affiliation:** Independent Researcher

## Overview

This project explores whether instructing a large language model (LLM) to answer only from a supplied passage can reduce unsupported answers.

The pilot compares two prompting methods:

1. **Normal prompting:** The model is asked to answer a question based on a passage.
2. **Grounded prompting:** The model is instructed to use only information explicitly stated in the passage and abstain when the answer is missing.

## Research Question

Does passage-grounded prompting help an LLM answer questions more reliably when the provided passage does not contain the requested information?

## Experimental Setup

- Model: Qwen/Qwen2.5-0.5B-Instruct
- Environment: Google Colab
- Dataset: 50 hand-authored question–passage pairs
- Evaluation: Manual comparison of model answers against the passage and expected answers
- Prompting conditions: Normal prompting and grounded prompting

## Dataset

The dataset contains answerable and unanswerable questions across several topics, including libraries, Mars, honeybees, solar panels, ancient Egypt, the Pacific Ocean, the Amazon rainforest, and the human heart.

The dataset is synthetic and is intended for a small pilot experiment, not as a validated benchmark.

## Results

Preliminary manual scoring is being used to compare the two prompting methods. The results should be treated as exploratory until the labels are independently checked.

See the research paper and experiment output files for the detailed methodology, responses, scoring, and limitations.

## Limitations

- Small, synthetic dataset
- One small instruction-tuned model
- Manual scoring that may involve reviewer judgment
- Limited number of experimental runs
- Results may not generalize to other models or real-world documents

## Reproducibility

The dataset and experiment notebook are provided for inspection and further testing. Model settings, prompts, scoring rules, and results should be checked before reproducing or extending the experiment.

## Research Integrity

This project is an educational pilot study. It does not establish that grounded prompting eliminates hallucinations in all LLMs. Any reported results should be interpreted within the limitations of the experiment.

## License

A license has not yet been selected. Please check the repository's intended reuse terms before adding one.
