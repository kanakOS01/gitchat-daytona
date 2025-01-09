This repository contains a README file sample for Daytona Samples and the MIT License.

It can be used as a template to create sample repositories that can be added into [Daytona](https://github.com/daytonaio/daytona).

Once you finish your sample and it gets merged, you can open a PR in the Daytona repo and submit the sample into the [index file](https://github.com/daytonaio/daytona/blob/main/hack/samples/index.json).

# Sample Streamlit with OpenAI & Weaviate

Git Chat is a RAG application that allows you to have a q/a session with any github repository of your choice. This is especially helpful for beginners who find it difficult to understand complex open source code bases on github.

It uses [Daytona](https://www.daytona.io/docs/) for managing environment, [weaviate cloud vector database](https://weaviate.io/) to store the embeddings, [LangChain with OpenAI](https://python.langchain.com/docs/) for llm models and facilitate queries with context and [streamlit](https://streamlit.io/) for UI.

---

## 🚀 Getting Started  

### Open Using Daytona  

1. **Install Daytona**: Follow the [Daytona installation guide](https://www.daytona.io/docs/installation/installation/).  
2. **Create the Workspace**:  
   ```bash  
   daytona create https://github.com/kanakOS01/gitchat-daytona.git
   ```
3. **Create a `.env` file**
   Get OpenAI API key from [here](https://platform.openai.com/api-keys).
   To setup Weaviate cluster url and api key refer [this](https://weaviate.io/developers/weaviate/quickstart).
   ```bash
   # openai api key
   OPENAI_API_KEY=""

   # weaviate configs
   WEAVIATE_CLUSTER_URL=""
   WEAVIATE_API_KEY=""
   ```
5. **Start the Application**:  
   ```bash  
   streamlit run gitchat/app.py
   ```
   Go to `https://localhost:8501` to view the application.

---
