# 🤗huggingFace🤗
learning hugging face
# Getting Started

if you are here you already know what huggingFace is. let's just work on it

## Required Base

To begin, ensure you have the following dependencies installed:

1. Python pip
2. PyTorch
3. Transformers

## Pipeline Examples

### Sentiment Analysis

You can perform sentiment analysis using the `pipeline` module from Transformers:

```python
from transformers import pipeline

classifier = pipeline("sentiment-analysis")
result = classifier("I love this jacket")

print(result)
```
### Text Generation

For text generation tasks, you can utilize the `pipeline` module with the appropriate parameters.

```python
from transformers import pipeline

generator = pipeline(task="text-generation", model="distilgpt2")
result = generator(
    "I love cars",
    max_length=40
)

print(result) 
```

### More Parameters

official [documentation](https://huggingface.co/docs/transformers/main/en/main_classes/pipelines#transformers.pipeline)
