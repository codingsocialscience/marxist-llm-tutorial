## Tutorial for Marxist Language Models

This tutorial expands [Nelimarkka's (2026)](https://journals.sagepub.com/doi/10.1177/20539517261447831) work on finetuning language models to make social science perspectives more prominent.

If you rather have a presentation, Matti has also produced a lecture on [Examining the worldviews embedded in LLMs](https://youtu.be/TNx7-eX96gY?si=MPyXW5fJkZdk2ReW) for Summer Institutes in Computational Social Science.

## Content

* `Inference.ipynb` Notebook shows how to load a foundation model using the transformers framework.
* `Finetune.ipynb` Notebook to finetune a model to be used yourself.
* `models/` contains the fine-tuned Marxist model

## Learning activity

### Before class
Install packages

``pip install transformers[torch] datasets torch ipywidgets pandas``

After that in the project folder

``hf download openai-community/gpt2``

### Workshop activity

We conduct quantitative content analysis by providing examples and then the message we wish to analyse.
The examples provide the classification scheme, here political (1) or not political (0).
One might come up with more examples here.
The two final lines contain the content to be classifier, most importantly `Label:` without a number.
The language model should pattern match and give this a number in the output.

```
Message: 'The new smartphone features a better camera and longer battery life.'
Label: 0
Message: 'The senator proposed a new bill to reform healthcare.'
Label: 1
Message: 'The local bakery is famous for its sourdough bread.'
Label: 0
Message: 'The government has announced new policies to improve the economy.'
Label:
```

> ⚠️ This way of doing content analysis seems to work with our limited _GTP2_-model.
> With more cutting edge models, the labelling task is usually given directly with elaborated codebooks rather than only examples like this.
> For more contemporary approach, see for example [Stuhler et al. (2025)](https://journals.sagepub.com/doi/full/10.1177/00491241251336794).

