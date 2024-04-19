# CS5246

## Organization in folders

- eda: Scripts and data for EDA
- generated: Scripts and data for data generation from models
- notebook: shared code for various tasks

## Data generation

Approach \#1 is to generate articles from our data source, each with top k keywords extracted for prompt formulation.

Each generation set is associated with a LLM and a specific format of prompt, such that output is expected to be more consistent.

3 LLMs were used, and the final dataset is in generated/cleaned folder
- `cleaned_microsoft_2.zip`- Phi-2 data
- `cleaned_mistral_2.zip`- Mistral data
- `data_generated_gpt_2.zip` - GPT data

Training the model is in folder `notebook/notebook_train.ipynb`
```
5-fold ROC AUC Score: 97.7%
```