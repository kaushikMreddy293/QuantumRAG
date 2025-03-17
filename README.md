# QuantumRAG: A Custom Retrieval-Augmented Generation Model

## Overview

QuantumRAG is a custom-built **Retrieval-Augmented Generation (RAG)** model designed to answer questions about quantum physics. It utilizes **FAISS** for document retrieval, **Hugging Face sentence embeddings** for vector similarity, and **Flan-T5** for answer generation.

## Features

- **Efficient Retrieval**: Uses FAISS to index and retrieve relevant knowledge chunks.
- **Advanced Embeddings**: Leverages `sentence-transformers/all-mpnet-base-v2` for document embeddings.
- **LLM-Powered Answers**: Uses `google/flan-t5-large` to generate concise and accurate responses.
- **Custom Prompt Engineering**: Structured prompts ensure high-quality responses.
- **Pydantic Validation**: Ensures structured outputs.

## Installation

To set up and run this project, follow these steps:

1. Download the Python Notebook
2. Run it on Google Collab or Jupyter Notebook
3. Get your API Key from Hugging Face 

### 4. Set Up Environment Variables

You need a **Hugging Face API token** to use the Hugging Face models. Set it up as follows:

```bash
export HUGGINGFACEHUB_API_TOKEN="your_huggingface_token"
```
For Windows:

```powershell
$env:HUGGINGFACEHUB_API_TOKEN="your_huggingface_token"
```

## Example Output

```txt
Question: Explain quantum mechanics in 15 words.
Answer: Quantum mechanics describes particles as probabilistic, exhibiting wave-particle duality, superposition, and entanglement.
--------------------------------------------------
Question: Describe the concept of entanglement in 15 words.
Answer: Entanglement links quantum particles, where measuring one instantaneously affects the other, regardless of distance.
--------------------------------------------------
```

## Dependencies

- `langchain`
- `transformers`
- `faiss-cpu`
- `pydantic`
- `sentence-transformers`
- `openai` (Optional, if using OpenAI models)


## Future Improvements

- Expand knowledge base with more topics.
- Improve retrieval quality with chunking strategies.
- Add API for external integrations.

## License

MIT License

---
