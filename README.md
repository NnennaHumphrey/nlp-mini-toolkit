# 🤖 NLP Mini Toolkit (FLAN-T5)

A simple Python project demonstrating core NLP tasks using **Hugging
Face Transformers** and **FLAN-T5**.\
Includes text generation, summarization, question answering, and basic
conversational AI.

------------------------------------------------------------------------

## Features

-   📝 Text generation\
-   📚 Summarization\
-   ❓ Question answering\
-   💬 Simple chatbot responses

------------------------------------------------------------------------

## Installation

``` bash
pip install transformers
```

------------------------------------------------------------------------

## Usage

``` python
from transformers import AutoTokenizer, AutoModelForSeq2SeqLM, pipeline

model_name = "google/flan-t5-small"
tokenizer = AutoTokenizer.from_pretrained(model_name)
model = AutoModelForSeq2SeqLM.from_pretrained(model_name)

generator = pipeline("text2text-generation", model=model, tokenizer=tokenizer)
result = generator("Complete this sentence: I want to")
print(result)
```

------------------------------------------------------------------------

## Project Structure

```text
├── .venv/                  
├── pretrained LLM.ipynb    
└── README.md               
```



------------------------------------------------------------------------

