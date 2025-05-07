# AGENTIC-RAG-APPLICATIONS

This repository contains a series of Jupyter notebooks that guide you through building sophisticated Retrieval Augmented Generation (RAG) applications using the concept of AI Agents. The lessons progress from fundamental components like Router Engines and Tool Calling to constructing a full Multi-Document Agent capable of reasoning over disparate information sources.

## Overview

The notebooks demonstrate how to create agents that can intelligently use tools to interact with and retrieve information from various documents. This goes beyond basic RAG by adding a layer of agentic reasoning that allows the AI to decide the best approach to answer a query based on the available tools and data.

The progression is structured as follows:

1.  **Lesson 1: Router Engine**
    * Learn how to set up a query engine that can route questions to different data sources or querying strategies based on the query's intent.
2.  **Lesson 2: Tool Calling**
    * Explore how to define and implement custom tools (like data retrieval or summarization) that your LLM-powered agent can call and utilize.
3.  **Lesson 3: Building an Agent Reasoning Loop**
    * Understand the core concepts of building an agent with a reasoning loop that enables it to choose and use the appropriate tool(s) to answer questions based on a single document.
4.  **Lesson 4: Building a Multi-Document Agent**
    * Extend the agent concept to handle multiple documents simultaneously. Learn how to set up tools for different documents and build an agent capable of navigating and synthesizing information across all of them.

## Repository Contents

* `L1_Router_Engine.ipynb`: Notebook covering the Router Engine concept.
* `L2_Tool_Calling.ipynb`: Notebook focusing on defining and using Tools for LLMs.
* `L3_Building_an_Agent_Reasoning_Loop.ipynb`: Notebook demonstrating how to build a single-document agent.
* `L4_Building_a_Multi-Document_Agent.ipynb`: Notebook showcasing the construction of a multi-document agent.
* `requirements.txt`: (Likely included in the helper/utils from the notebooks, but good practice to list requirements) - *You might need to create/verify this file based on notebook imports.*
* `data/`: Directory containing the documents used in the notebooks (e.g., `metagpt.pdf`, etc.). - *Ensure this directory and files are present in your repo.*
* `helper.py`, `utils.py`: (If used as indicated in notebooks) Helper scripts. - *Ensure these files are present in your repo.*

## Setup and Installation

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/sarankumar1325/AGENTIC-RAG-APPLICATIONS.git](https://github.com/sarankumar1325/AGENTIC-RAG-APPLICATIONS.git)
    cd AGENTIC-RAG-APPLICATIONS
    ```
2.  **Create a virtual environment (recommended):**
    ```bash
    python -m venv venv
    source venv/bin/activate # On Windows use `venv\Scripts\activate`
    ```
3.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
    *(Note: You might need to create the `requirements.txt` file based on the libraries used in the notebooks if it's not already in the repo.)*
4.  **Set up API Keys:**
    * The notebooks likely use an LLM API (e.g., OpenAI). You will need to set up your API key. Follow the instructions in the notebooks or helper files regarding API key configuration (e.g., using environment variables or a `.env` file).

5.  **Run the Notebooks:**
    ```bash
    jupyter notebook
    ```
    Open the `.ipynb` files in your browser to follow the lessons.

## Concepts Covered

* Retrieval Augmented Generation (RAG)
* AI Agents
* Tool Calling for LLMs
* Agent Reasoning Loops
* Router Query Engines
* Multi-document querying and synthesis
