# Hi, I'm Mohammad Mahdi Assaf

Final-year CS student at the Lebanese University, graduating July 2027. I build Python backends for LLM systems: MCP servers, retrieval, agents and evals. Each project ships with tests, CI, and numbers I measured myself.

## What I'm building

- 📚 **[STUDYSYSTEM](https://github.com/mohammadmassaf/STUDYSYSTEM)**: an MCP server that plans my semester across all 8 of my courses. It takes in past exams and lecture material, then ranks each evening's study plan by exam weight, how weak I am on each topic, and how close the exam is. The server never calls a model: the host (Claude) generates through a two-tool contract, and the server stores, validates and schedules, keeping only output that passes its schema. 21 tools, SQLAlchemy Core + Alembic, SQLite with Postgres proved in CI, FSRS spaced repetition. Milestone 1 shipped October 2026 and I study off its plan; v1 lands 30 November.
- 🔨 **[Grounded Forge](https://github.com/mohammadmassaf/GroundedForge)** · **▶ [Try it live](https://huggingface.co/spaces/mohammad778/grounded-forge)**: a cite-or-strike artifact generator. Every claim cites your own documents, and an independent Critic agent strikes anything the sources don't support. Study mode turns course PDFs into a cited quiz; job mode turns git history and project notes into cited CV bullets and STAR answers. **100% grounding on study mode (40/40 claims), 96.7% on job mode (29/30), 100% recall@10, 6/6 inflation traps caught** (`openai/gpt-oss-20b`, August 2026). Hand-rolled multi-agent loop, hybrid retrieval (BM25 + RRF + cross-encoder re-rank), 232 tests + CI, Docker image that runs with no network at all.
- 🍽️ **[MealWise](https://github.com/mohammadmassaf/mealwise)** · **▶ [Live demo](https://mealwise-iota.vercel.app)**: AI meal-planning app. LLM-generated multi-day plans with nutrition verified against the USDA food database. FastAPI backend, JWT auth.

## Stack

- **Languages:** Python (primary), Java, C, JavaScript, SQL
- **Backend:** FastAPI, SQLAlchemy, Alembic, SQLite, PostgreSQL, pytest, GitHub Actions, Docker
- **AI:** MCP, RAG, hybrid retrieval, multi-agent loops, LLM evaluation
- **Courses:** CS50x & CS50P (Harvard), Anthropic Academy

## Reach me

- LinkedIn: [mohammad-assaf](https://www.linkedin.com/in/mohammad-assaf-1b9668349)
- Email: mohammadmassaf1@gmail.com
