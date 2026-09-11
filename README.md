<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/banner.svg">
  <source media="(prefers-color-scheme: light)" srcset="./assets/banner-light.svg">
  <img src="./assets/banner.svg" width="860" />
</picture>

<br>

I build backend systems, ML pipelines, and the harnesses that make AI agents actually useful. I spec it, ship it, break it, fix it — then let the agents handle the rest. Based in Spain.

---

### Skills

**AI Tooling / Workflow**

`Spec-Driven Development` `Harness Engineering` `MCP (Model Context Protocol)` `RAG Pipelines` `Agentic Coding`

**Systems / Languages**

[![Systems](https://skillicons.dev/icons?i=c,bash,linux,git,python,java,ts)](https://skillicons.dev)

**ML / AI**

`XGBoost` `scikit-learn` `MLflow` `Optuna` `Evidently AI` `LLMs` `LLM tool-calling`

**Backend**

[![Backend](https://skillicons.dev/icons?i=spring,fastapi,postgres,mongodb,redis,kafka,docker,aws,rabbitmq,prometheus,grafana,supabase,firebase&perline=7)](https://skillicons.dev)

**Web**

[![Web](https://skillicons.dev/icons?i=react,flutter,tailwind)](https://skillicons.dev)

---

### Projects

**[Konjo](https://konjo.com.es)** &nbsp; ![Status](https://img.shields.io/badge/In%20Progress-f59e0b?style=flat-square) &nbsp; *Coming soon to Google Play*

Productivity apps are built for neurotypical brains: they punish a missed day, show every feature on first launch, and turn streaks into guilt. Konjo (根性, *quiet determination*) is designed around ADHD instead — calm by default, features that appear when you need them, gentle rescue prompts when you're stuck, and a Momentum Mode that splits a task into micro-steps you take one at a time. Offline-first: SQLite on the phone is the source of truth, with throttled delta sync of 14 entity types to a Spring Boot backend and a conflict log kept on the device. Event-sourced XP with 69 achievements, health data correlated with a productivity score, Flyway migrations V1–V18, and CI/CD shipping an arm64 image to Oracle Cloud. Built with Spec-Driven Development, plus a RAG over the project's 240K tokens of specs that I serve to the coding agent through an MCP server — 72% fewer tokens than loading the right spec, 15/15 retrieval hits.

`Java 21` `Spring Boot 3.5` `PostgreSQL 17` `Redis` `Flyway` `React Native` `Expo` `TypeScript` `SQLite` `React` `Vite` `Testcontainers` `RAG` `MCP`

**[A-Maze-ing](https://github.com/jzelada97/a-maze-ing)** &nbsp; ![Status](https://img.shields.io/badge/Completed-22c55e?style=flat-square) &nbsp; [**Play it**](https://maze.zelada.es)

A maze generator that you can also walk through. Two kinds of board come out of one pipeline, chosen by a single config key: a *perfect* maze — a spanning tree, exactly one route between any two cells — or a braided Pac-Man board with no dead ends at all. Algorithms are pluggable through a Strategy registry, and the generator ships as an installable wheel that depends on nothing else in the repo. The web layer on top is deliberately a *neighbour* of the graded project, not an extension of it: the engine gains no FastAPI import and the quality gate never runs a line of it. FastAPI with SSE streaming, a canvas you steer with the arrow keys, and a chat with tool-calling that drives the whole thing in plain language. 300+ tests behind one `make qa`.

`Python 3.12` `FastAPI` `SSE` `Pydantic` `pytest` `mypy --strict` `LLM tool-calling` `Docker`

**[HR Insights ETL](https://github.com/jzelada97/hr-insights-etl)** &nbsp; ![Status](https://img.shields.io/badge/Completed-22c55e?style=flat-square) &nbsp; [**Try it**](https://hr.zelada.es)

Kafka emits fragments of a person — personal, banking, location, professional — and not one of them carries an ID. This rebuilds the whole record on the other side. Medallion architecture: MongoDB keeps the raw message untouched (Bronze), Redis buffers fragments by match key with a TTL, PostgreSQL holds the consolidated record (Gold). The real work is the reconciliation engine — priority matching on passport, then normalised name, then address, with a fuzzy rule that demands corroboration, because without it two namesakes merge into a person who does not exist. Rewrote the exact-name pass from an O(n²) self-join into set operations to make it finish at all. 92% of the code is mine.

`Python` `Kafka` `MongoDB` `Redis` `PostgreSQL 16` `SQLAlchemy 2` `Pydantic 2` `FastAPI` `Streamlit` `Prometheus` `Docker Compose`

**[SentiLife](https://github.com/jzelada97/SentiLife)** &nbsp; ![Status](https://img.shields.io/badge/Completed-22c55e?style=flat-square)

Elderly people fall and no one knows for hours — we fixed that. Event-Driven platform that detects falls in real time. I led the backend using Spec-Driven Development: designed the specs, let agents generate the scaffolding, then built the real logic — REST APIs with Spring Security + JWT, async Virtual Threads, RabbitMQ messaging, and full observability (Prometheus + Grafana). Deployed on AWS with CI/CD via GitHub Actions.

`Java 21` `Spring Boot 3` `RabbitMQ` `PostgreSQL` `Docker` `AWS` `Prometheus` `Grafana` `Python` `GitHub Actions` `SDD`

**[ClaimVox](https://github.com/jzelada97/claimvox)** &nbsp; ![Status](https://img.shields.io/badge/Team%20project-6366f1?style=flat-square)

Multiclass classification of written financial complaints (CFPB, 1.9M rows) into eleven product families, where the model proposes and a person always decides — human review is mandatory even when confidence is high. My slice was the backend: the FastAPI foundation, JWT auth, Docker packaging, feedback persistence in PostgreSQL under least privilege, and the AWS deploy.

`Python` `FastAPI` `scikit-learn` `PostgreSQL` `Docker` `AWS` `JWT`

**[Housing Price Predictor](https://github.com/jzelada97/housing-price-predictor)** &nbsp; ![Status](https://img.shields.io/badge/Completed-22c55e?style=flat-square)

Madrid housing prices are opaque — listings don't reflect real market value. Built an XGBoost model with a full MLOps pipeline: automated hyperparameter tuning with Optuna, experiment tracking in MLflow, data drift monitoring with Evidently AI, and one-click deployment on Render.

`Python` `XGBoost` `MLflow` `Optuna` `Evidently AI`

**42 School** — Low-level C projects: [push_swap](https://github.com/jzelada97/push_swap) · [so_long](https://github.com/jzelada97/so_long) · [pipex](https://github.com/jzelada97/pipex) · [minitalk](https://github.com/jzelada97/minitalk) · [ft_printf](https://github.com/jzelada97/ft_printf) · [get_next_line](https://github.com/jzelada97/get_next_line) · [libft](https://github.com/jzelada97/libft)

**42 School** — Python: [Python Modules](https://github.com/jzelada97/ModulosPython) — 11 progressive modules from OOP to design patterns, Pydantic v2, and functional programming.

---

### Find me

<a href="mailto:josecarloszv97@gmail.com">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="./assets/gmaildark.svg">
    <source media="(prefers-color-scheme: light)" srcset="./assets/Gmail-Light.svg">
    <img src="./assets/gmaildark.svg" width="32" height="32" />
  </picture>
</a>
&nbsp;
<a href="https://www.linkedin.com/in/jzeladadev/">
  <img src="./assets/LinkedIn.svg" width="32" height="32" />
</a>
&nbsp;
<a href="https://zelada.es">
  <img src="./assets/webicon.svg" width="138" height="32" />
</a>
