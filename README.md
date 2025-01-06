This is an agentic RAG (Retrieval-Augmented Generation) application where the model responds to queries using specific data stored in a vector database.

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
