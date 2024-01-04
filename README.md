# Handkerchief
## Overview
Handkerchief is the classy and sophisticated alternative to RAG. Stop being GPU-poor and give openai your money by shoving your entire text corpus into parallelized gpt-3.5-turbo-16K calls! Handkerchief does everything you want:
- ✅ Misses less information
- ✅ Understands more of the surrounding context
- ✅ Gives better answers when nothing is found
- ✅ Uses more GPU's!!

## Installation
To use `handkerchief.py`, run:
```bash
pip install openai tiktoken
```
Get your [API Key](https://platform.openai.com/docs/api-reference/authentication#:~:text=The%20OpenAI%20API%20uses%20API%20keys%20for%20authentication.%20Visit%20your%20API%20Keys%20page%20to%20retrieve%20the%20API%20key%20you%27ll%20use%20in%20your%20requests.) and add this line to your `~/.bashrc` or `~/.zshrc`
```bash
export OPENAI_API_KEY='your-api-key'
```

## Usage
See the `test()` function for an example of running handkerchief. RAG is implemented with `handkerchief.sneeze()`, which does two things:

1. It searches through all 15K token chunks of text for relevant information.
2. It generates a response based on the information found.

**NOTE**: The prompts used in the script are just examples. You should engineer the prompts to suit your specific use case.

---
made by Ivan Yevenko
