# CS5246

## Folders
- eda: Scripts and data for EDA
- generated: Scripts and data for data generation from models
- notebook: shared code for various tasks

## Data generation

Approach \#1 is to generate articles from our data source, each with top k keywords extracted for prompt formulation.

Each generation set is associated with a LLM and a specific format of prompt, such that the output is more consistent.

All  generation sets each is denoted with a suffix character on paths.

- `x` - Pretrained AutoModelForCausalLM from Hugging Face Transformers library, named "mistralai/Mistral-7B-Instruct-v0.1"
