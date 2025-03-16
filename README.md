# 🏢 AI-Powered Multi-Agent RAG with AstraDB & Wikipedia Search  

## 🚀 Project Workflow

<img src="https://github.com/akankshakusf/Multi-Agent-Langraph-with-AstraDB/blob/master/MultiAgentProjectLayout.svg" width="100%" />

## 🔄 Workflow: AI-Powered Multi-Agent RAG System  

1️⃣ **User Input**: The user submits a query API request.  

2️⃣ **AI Query Routing**:  
   - The request is processed by an **AI Query Router**.  
   - The router determines whether to search in a **vector database (AstraDB)** or use **Wikipedia search** as a fallback.  

3️⃣ **Embedding Generation (Hugging Face)**:  
   - If querying **AstraDB**, the input is converted into **vector embeddings** using **Hugging Face models** for **semantic search**.  

4️⃣ **Retrieval Agents Work**:  
   - 🔍 **Agent1 (Wikipedia Search)**: Queries **Wikipedia** if the information isn’t in AstraDB.  
   - 🏛 **Agent2 (AstraDB + Cassandra)**: Retrieves the most relevant **vector embeddings** if a match is found.  

5️⃣ **Response Synthesis (Groq LLM)**:  
   - The retrieved data (from **AstraDB or Wikipedia**) is sent to **Groq LLM**.  
   - The **LLM applies prompt engineering** to generate a refined, human-like response.  

6️⃣ **AI Response to User**:  
   - The **final response is delivered** to the user via the **Streamlit UI or API output**.  


## 🔥 Why Enterprises Need This  

Today's organizations **generate massive unstructured data**—emails, PDFs, research papers, compliance documents, and internal reports. However, **90% of this data remains unread and unutilized** due to a lack of efficient retrieval mechanisms.  

This project solves that problem with an **AI-driven, multi-agent retrieval system** powered by **AstraDB (Cassandra-based vector storage) and Wikipedia Search**, enabling enterprises to:  
✅ **Instantly access** relevant insights from corporate data.  
✅ **Analyze millions of unread documents** in seconds.  
✅ **Combine private & public knowledge** seamlessly.  
✅ **Enhance decision-making** with AI-driven retrieval.  

### **🚀 The Future of AI-Powered Search in Enterprise**  
Traditional databases fail to handle **semantic search** effectively. Instead of manually tagging documents, we **convert all knowledge into embeddings** and store them in **AstraDB**, a scalable **vector database**.  

- **🔹 Replace Vector Store with Enterprise Data Lakes**  
  - Enterprises store **billions of raw documents** in **data lakes (AWS S3, Azure Data Lake, Google Cloud Storage)**.  
  - These files are often **unstructured and inaccessible** to traditional SQL queries.  
  - Using this approach, companies can **convert documents into vector embeddings** and **store them in AstraDB or any vector database**.  
  - AI agents can then **retrieve the most relevant context within seconds**, reducing **manual research hours to milliseconds**.  

- **🔹 Agents as Intelligent Knowledge Workers**  
  - A **retrieval agent** queries AstraDB first.  
  - If no relevant data is found, the agent **autonomously routes the query** to external sources like Wikipedia or enterprise APIs.  
  - This eliminates **blind spots** and ensures access to **both private & public knowledge**.  
