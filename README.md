# GDC Project Chatbot

A simple chatbot designed to answer natural language queries related to GDC Projects.

## Background

When students applied for GDC Projects, myself included, they faced challenges navigating the available opportunities. The original Word document contained over 70 projects but had no efficient way to:

1. Understand project details as the document listed only companies/research labs' names, and users had to click individual links to find out what each project was about
2. Search for relevant projects based on specific interests, required skills, or research domains.
3. Quickly filter projects based on personal preferences, which ultimately lead to a time-consuming and sometimes disorganized application process.
## Solution

<img width="959" alt="Pasted image 20250204141041" src="https://github.com/user-attachments/assets/210ff086-87fa-4d2e-8c14-ee0cc5e86e88" />

To address this, I built a chatbot that allows students to:

✅ **Receive project summaries** – Get clear, concise information about relevant projects without having to sift through the entire document.  
✅ **Improve decision-making** – Quickly identify projects aligned with their career and learning goals.
✅ **Search projects using natural language** – Ask about projects related to specific topics, skills, or keywords.  
## How It Works (RAG-based Approach)

1. **Data Preparation** -- Converted tabular CSV data into structured natural language descriptions using paragraph templates 
2. **Precomputed Embeddings** -- Used Gemini embedding model and saved them privately for confidentiality
3. **Retrieval Step** -- Input queries are converted into embeddings and cosine similarity is used to retrieve top 10 most relevant projects 
4. **Response Generation** -- A large language model (i.e., Gemini) then uses the retrieved project descriptions as context to generate response to the query
## Usage

Visit the Hugging Face Space to access the chatbot:

https://huggingface.co/spaces/jonwibowo/GDC_Chatbot

⚠ Note: This chatbot is no longer actively maintaining the chatbot since application period is over
