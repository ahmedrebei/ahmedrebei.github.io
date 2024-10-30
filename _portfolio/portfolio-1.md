---
title: "Quebec Consultant Multi-Agent Chatbot"
excerpt: "The Multi-Agent Chatbot project leverages multiple agents, including the Retrieval Agent (RAG), to provide accurate and comprehensive answers to user questions about topics related to immigration or education in Quebec. The chatbot is able to retrieve relevant information from a knowledge base and deliver informative responses. <br/><img src='/images/chatbot.png'>"
collection: portfolio
---

## Overview

The Multi-Agent Chatbot project leverages multiple agents, including the Retrieval Agent (RAG), to provide accurate and comprehensive answers to user questions about topics related to immigration or education in Quebec. The chatbot is able to retrieve relevant information from a knowledge base and deliver informative responses.


## Project Structure

```
consultant_bot
├── agents
│   ├── agent.py
│   ├── generator_agent.py
│   ├── grading_agent.py
│   ├── greeting_agent.py
│   ├── retrieval_agent.py
│   └── summarization_agent.py
├── data
│   ├── chroma_data
│   ├── chroma_store.py
│   ├── data.json
│   ├── links.json
│   └── scrapper.py
├── config.py
├── Dockerfile
├── README.md
├── requirements.txt
├── run.py
└── workflow.py

```

### Files Description

### Files Description

- **README.md**: The main documentation file for the project.
- **agents**: A directory that contains the implementation of different agents used in the chatbot, including:
    - **agent.py**: Generic agent class that serves as the base for other specialized agents.
    - **generator_agent.py**: Generation agent class.
    - **grading_agent.py**: Grading agent class.
    - **greeting_agent.py**: Greeting agent class.
    - **retrieval_agent.py**: RAG agent class.
    - **summarization_agent.py**: Summarization agent class.

- **config.py**: Get API_KEY from `.env` file.
- **data**: Contains data related files:
    - **chroma_data**: Directory when Chroma stores the vector store.
    - **chroma_store.py**: Vector store class.
    - **scrapper.py**: scrapping class to scrap input links from `links.json` and store the ouput in `data.json`
    - **data.json**: Data.
    - **links.json**: Links to scrap.
- **requirements.txt**: List of all the dependencies.
- **workflow.py**: The workflow class of the chatbot.
- **run.py**: The main entry point for running the streamlit application.
![chatbot](/images/chatbot.png)