# LLM-Hallucination-Demo

## What the project does:
This is a demonstration project to show the power of the ChatGPT LLM to summarize, analyze and refine a biomedical literature/citation search. The project uses the concept of in-context learning to overcome LLM hallucination and also allows the LLM to work with information post its training and deployment dates. 
A keyword search of the PubMed biomedical literature database is conducted to retrieve the information to create an in-context learning string. The ChatGPT API is then used with a refined prompt to summarize  and provide a report of the keyword search. 
This is a simple form of in-context learning demonstration. No embedding/vector databases are used in this demonstration.

## Why the project is useful:
Hallucination, defined as an answer to a prompt that sounds reasonable, but is factually inaccurate or untrue.  Hallucination is a key stumbling block to trust and adoption of LLM and is especially problematic in mission critical type or other use cases, such as found in the biomedical field, where ground truth is vitally important.
Here is what ChatGPT has to say about hallucination:

      ‘Hallucination is a phenomenon that occurs in large language models (LLMs) and refers to their tendency to generate outputs that may appear plausible but are not               factually accurate or grounded in reality. It is a significant limitation that researchers and scientists in the field are actively working to address.’

This project shows how the Biopython and ChatGPT APIs can be used to create an in-context learning string to help address LLM hallucination. In this simple form of in-context learning we pre-process or curate the data provided through a PubMed citation search. While still limited by the  token number, we provide a solid grounding and context to the LLM, address hallucination without requiring large amounts of compute time.

## How users can get started with the project:
The project repository is in the form of a Jupyter notebook. It was created within the Anaconda data science development platform. In order to access the ChatGPT API, you will need to create an account with OpenAI and obtain an API key. The python libraries needed in your development environment are listed below.

   Anaconda: https://www.anaconda.com/

  Python Libraries:

  * openai: https://platform.openai.com/docs/api-reference
  * tiktoken: https://github.com/openai/tiktoken
  * BioPython: https://github.com/biopython/biopython/blob/master/README.rst
  * dotenv: https://github.com/theskumar/python-dotenv#getting-started
