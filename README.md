# Custom Knowledge Chatbot (LlamaIndex)

A minimal retrieval-augmented chatbot: load your own documents, index them with LlamaIndex + OpenAI embeddings, and ask questions answered from that content.

## How it works
1. Documents in `neet/data/` are loaded and chunked
2. A `VectorStoreIndex` is built with an OpenAI-backed `ServiceContext`
3. `index.as_query_engine()` answers natural-language questions grounded in the docs

## Run
```bash
pip install -r neet/requirements.txt
export OPENAI_API_KEY=your-key
jupyter notebook "neet/Custom Knowledge Chatbot.ipynb"
```

## Credits
Based on Liam Ottley's [Custom Knowledge Chatbot with LlamaIndex](https://www.youtube.com/@LiamOttley) tutorial.
