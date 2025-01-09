# RAG-System-Langchain
This notebook demonstrates the implementation of a **Retrieval-Augmented Generation (RAG)** system using LangChain and an open-source LLM  **Flan-Alpaca GPT-4**. The RAG approach enhances large language models (LLMs) by integrating external knowledge, enabling them to generate accurate and contextually relevant responses

## **Implementation:**

**1. Data Ingestion from PDF Files:**

  * Reads data from one or more PDF files.

  * Processes the text content for use in downstream tasks.

**2. Vector Store for Knowledge Storage:**

 * Converts the extracted textual data into embeddings (dense numerical representations).

 * Stores these embeddings in a vector store, enabling efficient similarity-based retrieval.


**3. LLM Query and Response:**

 * Uses LangChain to interact with the vector store and retrieve relevant information based on user queries.

 * Combines retrieved information with the LLM to generate a response, ensuring the model is informed by the external knowledge.
 * Also Provides Reference of response from the given Data


## **Workflow**

**1. Data Preparation:**

* Extract text from PDF files and process it into a usable format.

**Embedding and Storage:**

* Create embeddings for text chunks and store them in the vector database.

**2. Query Handling:**

* Accept user queries.

* Retrieve the most relevant chunks from the vector store using similarity search.

* Pass the retrieved context along with the query to the LLM.

**3. Response Generation:**

* The LLM generates a response, informed by the retrieved data, to ensure relevance and accuracy.


By combining the capabilities of LangChain and open-source LLMs with a robust vector storage mechanism, this implementation ensures efficient and accurate query resolution in diverse domains.

## **Citation :**
1. Introduction | 🦜️🔗 LangChain. (n.d.). Introduction | 🦜️🔗 LangChain. https://python.langchain.com/docs/introduction/
2. Hugging Face - Documentation. (n.d.). Hugging Face – The AI community building the future. https://huggingface.co/docs
3. GitHub - declare-lab/flan-alpaca: This repository contains code for extending the Stanford Alpaca synthetic instruction tuning to existing instruction-tuned models such as Flan-T5. (n.d.). GitHub. https://github.com/declare-lab/flan-alpaca
4. GitHub - huggingface/optimum: 🚀 Accelerate inference and training of 🤗 Transformers, Diffusers, TIMM and Sentence Transformers with easy to use hardware optimization tools. (n.d.). GitHub. https://github.com/huggingface/optimum
5. Chroma Docs. (n.d.). Chroma Docs. https://docs.trychroma.com/docs/overview/introduction
