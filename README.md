# Too Long; Don't Read
> # [toolongdontread.live](https://toolongdontread.live)  

![Screenshot](/frontend/screenshot.png "Screenshot")

## Introduction

This is a text summarizer web app that is attached to a large language model, specifically flan-t5-small, fine-tuned to generate short TL;DR summaries of any text.

## Training
[Huggingface🤗 Repository](https://huggingface.co/zaydzuhri/flan-t5-base-tldr-100k)  
The flan-t5-base model was trained on a dataset of 100 thousand Reddit posts that contained a tl;dr summary in the comments, obtained from [this dataset](https://zenodo.org/record/1168855#.ZB8P-iFByUk). The model was trained for 5 epochs using the [Huggingface](https://huggingface.co/) [Transformers](https://github.com/huggingface/transformers) library. The model was trained on AWS Sagemaker using a g4dn.xlarge instance for ~12 hours.


## Usage

1. Open your browser and go to toolongdontread.live, or run frontend/index.html locally.
2. Paste the text you want to summarize in the input box.
3. Click on the "TL;DR" button.
4. The summary will be displayed below the input box.


## Acknowledgments

This project was heavily inspired by and follows the training setup from [this tutorial](https://www.philschmid.de/fine-tune-flan-t5)
