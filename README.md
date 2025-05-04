# llama-book-recommender

An AI-powered book recommendation system that matches user preferences to books using semantic similarity. This project combines transformer-based sentence embeddings with a LLaMA language model to deliver intelligent, personalized book suggestions.

## 🚀 Features
- Embeds book descriptions using `sentence-transformers` (`all-MiniLM-L6-v2`)
- Accepts natural language book descriptions as input
- Finds top-N similar books based on cosine similarity
- Uses Hugging Face's LLaMA model for enhanced language understanding

## 🧠 How It Works
1. **Dataset Loading**: Reads a curated dataset of popular books including titles, genres, and descriptions.
2. **Embedding Generation**: Transforms each book’s description into a vector embedding using a MiniLM model.
3. **User Query Input**: Takes a description of the type of book the user is looking for.
4. **Semantic Matching**: Compares the input embedding to book embeddings using cosine similarity.
5. **Top Picks**: Recommends the top 5 most relevant books.

## 🔗 Dataset Source
This project uses the ["Goodreads Best Books Ever"](https://www.kaggle.com/datasets/arnabchaki/goodreads-best-books-ever) dataset from Kaggle, created by [Arnab Chaki](https://www.kaggle.com/arnabchaki).

## 🛠️ Tech Stack
- Python
- [Transformers (Hugging Face)](https://huggingface.co/docs/transformers/index)
- [Sentence Transformers](https://www.sbert.net/)
- PyTorch with CUDA support
- Google Colab for execution


