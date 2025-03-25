# Fine-Tune LLMs Repository

This repository contains multiple language models, their fine-tuned versions, tokenizers, and related experiment files.

## Repository Structure

```
.
├── models/
│   ├── model1/
│   │   ├── data/                  # Data specific to model1
│   │   │   ├── raw/               # Raw data for training
│   │   │   └── processed/         # Preprocessed data for model1
│   │   ├── pretrained/            # Pretrained model1 files
│   │   ├── finetuned/             # Fine-tuned model versions
│   │   │   ├── resultsv1/         # First version of fine-tuned model
│   │   │   └── resultsv2/         # Second version of fine-tuned model
│   │   ├── tokenizer/             # Tokenizer files for model1
│   │   └── experiments/           # Experiment notes, metrics, etc.
│   │
│   ├── model2/
│   │   ├── data/                  # Data specific to model2
│   │   │   ├── raw/               # Raw data for training
│   │   │   └── processed/         # Preprocessed data for model2
│   │   ├── pretrained/            # Pretrained model2 files 
│   │   ├── finetuned/             # Fine-tuned model versions
│   │   │   ├── resultsv1/         # First version of fine-tuned model
│   │   │   └── resultsv2/         # Second version of fine-tuned model
│   │   ├── tokenizer/             # Tokenizer files for model2
│   │   └── experiments/           # Experiment notes, metrics, etc.
│   │
│   └── ...                        # Additional models
│
├── scripts/                       # Utility scripts for training, evaluation, etc.
├── notebooks/                     # Jupyter notebooks for exploration and visualization
└── configs/                       # Configuration files for training runs
```

## Usage

### Adding a New Model

To add a new model to the repository, create a new directory using the same structure:

```bash
mkdir -p models/new_model_name/{data/{raw,processed},pretrained,finetuned/{resultsv1,resultsv2},tokenizer,experiments}
```

### Working with Models

1. Store raw training data in the respective model's `data/raw/` directory
2. Place processed data ready for training in `data/processed/`
3. Maintain the pretrained model in the `pretrained/` folder
4. Save fine-tuned model versions in `finetuned/resultsv#/` directories
5. Keep tokenizers and related files in the `tokenizer/` directory
6. Document experiments, metrics, and results in the `experiments/` folder

## Requirements

List of dependencies and requirements for running the models.

## License

Add your license information here. 