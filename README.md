
# AI Knowledge Worker using FAISS

A Jupyter Notebook demo showing how to build a simple “knowledge worker” that:

1. Ingests documents (PDFs, text, etc.)  
2. Converts them into vector embeddings  
3. Stores and queries them with Facebook’s FAISS  
4. Uses an LLM to answer natural-language questions

---

## Features

- **Document ingestion**: Load files from disk or a folder.  
- **Embeddings**: Leverage OpenAI (or another) embedding model.  
- **Vector store**: Build and persist a FAISS index.  
- **Retrieval + QA**: Pull relevant text chunks and feed them to an LLM for answers.  
- **Interactive notebook**: Walk through each step, tweak parameters, and experiment.

---

## 🛠Getting Started

1. **Clone this repo**  
   ```bash
   git clone https://github.com/Rishi-Kora/AI-Knowledge-Worker-using-FAISS.git
   cd AI-Knowledge-Worker-using-FAISS


2. **Create a Python environment**

   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```

3. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Set your OpenAI API key**

   ```bash
   export OPENAI_API_KEY="your_api_key_here"
   ```

5. **Run the notebook**

   ```bash
   jupyter lab
   ```

   Open `AI Knowledge Worker using FAISS.ipynb` and follow along!

---

## How it works

1. **Load documents** into memory and split into chunks.
2. **Embed** each chunk with an embedding model.
3. **Build** a FAISS index on those embeddings.
4. **Query** the index with a new question, retrieve top-k similar chunks.
5. **Prompt** the LLM with retrieved context to generate the final answer.

---

## Contributing

Feel free to open issues or submit pull requests! Whether it’s:

* Adding support for more file types
* Swapping in a different embedding model
* Improving indexing or query performance

We’ll happily review and merge.

---

## 📄 License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.

