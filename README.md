# PubMed-LLM 

[![Python 3.11](https://github.com/andreaxricci/PubMed-LLM/actions/workflows/main.yml/badge.svg)](https://github.com/andreaxricci/PubMed-LLM/actions/workflows/main.yml)

## How does it work?

When the user inputs a question, the system triggers a PubMed search, enhancing the user input with the context of the conversation.

If results are found, the system leverages a LLM to provide a summarised answer based on the abstracts of the relevant articles, along with the references to them.

The screenshot below shows an example of the frontent, built with Streamlit:

<img width="1269" alt="Screenshot 2023-07-02 at 17 58 37" src="https://github.com/andreaxricci/PubMed-GPT/assets/62494809/4656cc78-079d-4a41-9530-691513959ef4">




In order to reproduce this, it is required to specify the following API keys in a .env file:

- OPENAI_API_KEY=... (Used for the LLM calls via Langchain)
- NCBI_API_KEY=... (Used for the metapub search. You can request one here: https://support.nlm.nih.gov/knowledgebase/article/KA-05317/en-us)

