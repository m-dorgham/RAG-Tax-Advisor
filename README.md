# Tax AI Assistant with LLM and RAG

Ever wished you had a tax expert on call to decode Germany's crazy-complicated tax laws? Yeah, me too! Today, we're going to build our very own AI tax assistant that can actually explain this stuff and answer our questions. Grab your coffee and let's get coding! 

### Technical Approach

- **Model Selection:** The system utilizes Qwen2.5, a high-performing, multilingual open-source decoder-based LLM, chosen for its balance of performance and efficiency. Specifically, I experimented with the 1.5B parameter variant, which is compact enough to run on a single GPU while maintaining strong multilingual capabilities.

- **RAG Pipeline:**

    - **Vector Store:** FAISS for efficient similarity search over embedded legal texts.

    - **Embedding Model:** granite-embedding-278m-multilingual (ranked among the top multilingual models on Hugging Face’s Embedding Leaderboard), selected for its optimal trade-off between multilingual performance and hardware efficiency.

    - **Document Processing:** LangChain for chunking, embedding, and storing legal documents in a retrievable format.

The `RAG-Tax-Advisor.ipynb` notebook documents the implementation and gives a step-by-step guide, providing a reproducible framework for building domain-specific AI assistants.

