# Recipe Generation with GPT-2

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1X0qB6o99g5L_YJ7Jp9HKzEWuPPn_64uz?usp=sharing)


This notebook explores how to fine-tune a transformer for a custom text completion task -- specifically, we'll teach GPT-2 to generate full recipe instructions from just a list of ingredients.

Before the world met ChatGPT, GPT-2 was already showing us what generative AI could do -- if we were paying attention. To learn more about this large language model, which was trained on 8 million web pages, check out the official model card on Hugging Face.

## The Roadmap

Before we get cooking, here's a roadmap of what is to come:

- Set up the GPU runtime
- Download and inspect the dataset
- Create a DataFrame and split it into training and test sets
- Test the base model on a single sentence
- Fine-tune the model using the recipe dataset
- Evaluate the fine-tuned model's recipe writing skills

## Tools & Libraries Used

- **Google Colab** — for free GPU access and seamless integration with Drive  
- **Python 3.12.7** — base language for all modeling and data wrangling  
- **pandas** — for reading and managing the dataset of 120K recipes  
- **transformers** — Hugging Face's library for working with GPT-2 and custom fine-tuning  
- **torch** — PyTorch backend powering the fine-tuning and inference  
- **curl** — to download the custom training script from the course server  
- **shutil** — for saving and exporting the fine-tuned model  
- **subprocess** — to manage training script execution with more readable output  
- **Google Drive** — used to store and export the final model

## Acknowledgements

This project began with a notebook I was working on for my NLP class, taught by  Associate Professor Michele Samorani at Santa Clara University. A tip of the cap to him and the Leavey School of Business for bringing these recipes to life.
