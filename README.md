# 🎓 Semester Starter Toolkit

**Goal:**  
This project is a teaching-oriented, open-source toolkit that grows step-by-step alongside a university course on **Python, data management, and modern retrieval systems**.  

The project demonstrates how to go from **basic Python logic** all the way to **advanced data curation, analytics, and semantic search with vector databases**, while solving practical problems students face at the beginning of a semester (organizing schedules, tracking assignments, managing budgets, searching syllabi).

It is organized into **modular prototypes**, each focused on one concept. Later, specialized "agents" (with defined roles) will integrate these pieces into a full solution.

---

## 🚀 Vision

By the end of this project we aim to have:

- A **student-facing CLI tool** that helps organize semester data (courses, assignments, budgets).  
- A **data management layer** built with CSV/JSON, Pandas, NumPy, and SQL.  
- A **retrieval layer** that ingests syllabi/notes, chunks and embeds them, and supports semantic + hybrid search with a vector DB.  
- A **visualization layer** for grade distributions, workloads, and budgets.  
- A **set of modular prototypes** that serve as learning artifacts and entry points for contributors.  

---

## 🧩 Prototypes (Learning Path)

Each prototype lives in `prototypes/` and is intentionally small, focused, and documented. Together, they cover the full stack of course topics.

### Core Python & Data Management
1. **00_env_smoke.py** – Environment sanity check  
2. **01_basic_python_logic.py** – Lists, dicts, loops, functions  
3. **02_regex_file_io.py** – File I/O and regex for text extraction  
4. **03_csv_json_roundtrip.py** – Reading/writing CSV and JSON  
5. **04_numpy_metrics.py** – Numeric operations and grade statistics  
6. **05_pandas_merge_clean.py** – Data cleaning and joining tables  
7. **06_matplotlib_charts.py** – Visualization (histograms, bar charts)  
8. **07_sqlite_schema_queries.py** – Relational DB schema and SQL queries  

### Vector DB & Retrieval (Extension Module)
9. **08_ingest_pdf_text.py** – Extract text from PDFs  
10. **09_chunker_basics.py** – Chunk text with metadata  
11. **10_embeddings_vector_search.py** – Embeddings + vector search  
12. **11_hybrid_search_bm25_vector.py** – Hybrid (keyword + vector) search  
13. **12_rag_stub_qna.py** – Prototype Q&A with citations  
14. **15_eval_retrieval_metrics.py** – Retrieval evaluation (Recall, MRR, nDCG)  

### Student-Facing Features
15. **13_semester_budget_tracker.py** – Track semester expenses & budgets  
16. **14_assignments_calendar_cli.py** – Assignment deadlines + calendar export  
17. **16_pipeline_orchestrator.py** – End-to-end orchestration script  
18. **17_logging_config_secrets.py** – Shared config & logging  
19. **18_privacy_redaction.py** – Redaction of PII before indexing  

---

## 🛠️ Tech Stack

- **Python 3.11+**
- **Core Data**: `pandas`, `numpy`, `matplotlib`
- **SQL**: `sqlite3` (stdlib), `sqlalchemy`, `duckdb`
- **File Handling**: `pypdf`, `pyyaml`
- **Vector DB / Retrieval**: `chromadb`, `sentence-transformers`, `rank-bm25`
- **CLI & UX**: `rich`, `ics`
- **Dev Tools**: `ruff`, `pytest`

---

## 📂 Project Structure

```
prototypes/        # individual prototype scripts
agents/            # role specifications (IO contracts)
data/samples/      # small CSV/JSON/PDF test files
docs/              # design notes, diagrams
notebooks/         # optional Jupyter exploration
src/               # shared library code (as it matures)
output/            # generated artifacts (gitignored)
```

---

## 🤝 How to Contribute

We welcome developers, educators, and students to join:

- **Fork & clone** the repo
- Create a feature branch (`git checkout -b feature/my-idea`)
- Add or improve a prototype
- Submit a Pull Request with clear description

**Ways to help:**
- Add new prototypes (e.g., CSV → Parquet converters, advanced visualizations)
- Improve retrieval accuracy (better chunking, embeddings, hybrid search)
- Write unit tests for prototypes
- Expand student-facing CLI functionality
- Contribute docs or teaching materials

---

## 🏃 Getting Started

1. Clone and set up environment:
   ```bash
   git clone https://github.com/<your-username>/semester-starter-toolkit.git
   cd semester-starter-toolkit
   python3 -m venv .venv
   source .venv/bin/activate
   pip install -r requirements.txt
   ```

2. Run the environment smoke test:
   ```bash
   python prototypes/00_env_smoke.py
   ```

3. Explore prototypes in order (see list above).

---

## 📜 License

This project is open source under the [MIT License](LICENSE).

---

## 🌟 Join Us

This is a learning-first, open-source project.  
If you’re passionate about **Python, data, teaching, or retrieval systems**, this is a place to experiment, contribute, and grow.  
Check out the issues tab for ideas or start a discussion!
