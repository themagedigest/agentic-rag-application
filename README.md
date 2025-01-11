This is an agentic RAG (Retrieval-Augmented Generation) application where the model responds to queries using specific data stored in a vector database.

<img width="137" alt="image" src="https://github.com/user-attachments/assets/c71d9459-94a3-41e7-9d7b-fbd3e7f87303" />


Agentic Architecture and Tech Stack:
1. Vector Database: Pinecone is utilized as the vector database, providing efficient storage and retrieval of relevant embeddings.
2. Model and Embeddings: OpenAI powers both the model and embedding generation for semantic understanding and accurate responses.
3. Orchestration Framework: LangGraph serves as an orchestration framework for managing complex agentic workflows.

Application Behavior:
The model exclusively generates responses based on the context retrieved from the Pinecone database. Queries outside the retrieved context are intentionally left unanswered to maintain accuracy and relevance.

Example Interaction:

User Query: What was Amazon.com's annual visitor count in 2008, and how much did it grow afterward?

Response:
In 2008, Amazon.com had 615 million annual visitors. By 2022, this figure grew to over 2 billion monthly visitors. Converting monthly visitors to an annual figure (2 billion × 12 months = 24 billion), the growth from 2008 to 2022 was approximately 23.385 billion additional visitors annually.
This architecture ensures precise, contextually grounded responses while avoiding irrelevant or speculative outputs.


Project Description: Agentic Retrieval-Augmented Generation (RAG) Application
This project involves building an agentic Retrieval-Augmented Generation (RAG) application designed to generate contextually grounded responses to user queries. The model leverages specific data stored in a vector database, ensuring high accuracy and relevance in its outputs.

Key Components:
Vector Database:

Utilized Pinecone as the vector database for efficient storage and retrieval of embeddings.
Pinecone enables fast and accurate access to relevant content for query resolution.
Model and Embeddings:

OpenAI's model is employed for both query understanding and embedding generation.
These embeddings allow semantic comprehension of data, enabling the model to provide precise answers.
Orchestration Framework:

LangGraph serves as the orchestration framework, managing the complex workflows required for the agentic behavior of the application.
Application Behavior:

The model exclusively generates responses based on context retrieved from the Pinecone database.
Queries outside the retrieved context are left unanswered to maintain the integrity and accuracy of the responses.
Example Interaction:
User Query: What was Amazon.com's annual visitor count in 2008, and how much did it grow afterward?
Response: In 2008, Amazon.com had 615 million annual visitors. By 2022, this figure grew to over 2 billion monthly visitors. Converting monthly visitors to an annual figure (2 billion × 12 months = 24 billion), the growth from 2008 to 2022 was approximately 23.385 billion additional visitors annually.

This ensures that the responses remain contextually relevant while avoiding speculation or irrelevant outputs.

Setup to follow -

1. Create a virtual environment - python3 -m venv virtual-env-name
2. Activate the virtual environment - source virtual-env-name/bin/activate
3. Install all the dependencies using the requirements.txt file - pip install -r requirements.txt
4. I have used Amazon.com company's wiki page.
6. I have used the pinecone database as my vector database. Create one account and start using it. Sign Up here - https://app.pinecone.io/
7. Keep your OPENAI_API_KEY and PINECONE_API_KEY handy.
