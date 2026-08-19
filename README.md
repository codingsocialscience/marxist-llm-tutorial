## Tutorial for Marxist Language Models

This tutorial expands [Nelimarkka's (2026)](https://journals.sagepub.com/doi/10.1177/20539517261447831) work on finetuning language models to make social science perspectives more prominent.

If you rather have a presentation, Matti has also produced a lecture on [Examining the worldviews embedded in LLMs](https://youtu.be/TNx7-eX96gY?si=MPyXW5fJkZdk2ReW) for Summer Institutes in Computational Social Science.


## Before class
Install packages

``pip install transformers[torch] datasets torch ipywidgets pandas``

After that in the project folder

``hf download openai-community/gpt2``

## Inference

Notebook shows how to load a foundation model using the transformers framework.

## Finetune

Notebook to finetune a model to be used yourself.
