# Hi, I'm Mikołaj

Data Engineer at Nokia and Systems Engineering student at Wrocław University of Science and Technology. Contributor in the [Robocik](https://www.robocik.pwr.edu.pl/) academic circle.

I build data pipelines and the infrastructure they run on. Currently focused on **RAG & LLM systems**, **MLOps**, **platform engineering** and my **homelab**.

[LinkedIn](https://www.linkedin.com/in/mikolaj-lepsy-6789892b4) · [mikolaj.lepsy@gmail.com](mailto:mikolaj.lepsy@gmail.com)

## What I've been working on

**[PM Generator](https://github.com/nokia-wroclaw/innovativeproject-pm-generator)** (Nokia Wrocław)
Generative pipeline for synthetic telecom Performance Management (KPI) data.
- PySpark preprocessing: gap imputation, KPI coverage filtering, greedy joint KPI selection, windowing of multivariate time series into training tensors
- Generative models (CVAE / LSTM) for multivariate KPI time series
- Orchestration with Airflow 3, FastAPI backend, Vue 3 UI for DAG management, fully Dockerized with devcontainers

**Graph databases** (Nokia)
Data engineering work with ArcadeDB and ArangoDB: loading and querying graph data from PySpark pipelines.

**Knowledge elicitation for RAG** (engineering thesis, in progress)
Pipeline that captures tacit expert knowledge and feeds it into RAG systems.

**[MusicaBI](https://github.com/LepsyMikolaj3301/MusicaBI)**
BI dashboard for music and artist data. End-to-end ETL with dlt, orchestrated in Airflow, deployed with Docker Compose, with tests.

**[factorio-RL-TowerDefense](https://github.com/LepsyMikolaj3301/factorio-RL-TowerDefense)**
Custom RL environment (`TowerDefenseEnv`) on top of the Factorio Learning Environment, where an agent defends a central radar against escalating enemy attacks by placing, supplying and managing turrets across ~20 perimeter slots.
- Environment: Dockerized headless Factorio servers driven over RCON, Lua server-side scripting, Gym-compatible Python wrapper (works with Stable-Baselines3, CleanRL, RLlib)
- Action space: ~81 discrete actions (move, place, pick up, resupply) with action masking; timing constraints solved analytically in the mask instead of learned
- Observations: dict space with obstacle and threat grids, per-slot turret features (ammo, health, threat, travel cost, coverage) and global state
- Model: MaskablePPO with a custom CNN + MLP feature extractor; next step is PPO-LSTM with a Deep Sets slot encoder

**[path_finders_comp](https://github.com/LepsyMikolaj3301/path_finders_comp)**
Interactive Dijkstra vs A* comparison on user-drawn maps (pygame).

**Homelab (in progress)**
Always-on home server, Tailscale networking, Wake-on-LAN and multi-hop SSH access to my workstation.

## Testing & QA project (in progress)

University testing course project, done as a two-person team on a fork of [NoteDiscovery](https://github.com/gamosoft/NoteDiscovery), an actively maintained FastAPI app with no existing test suite.
- Unit and integration tests with pytest, run in GitHub Actions
- End-to-end browser tests with Playwright, plus structured user testing
- Contributing the useful parts back upstream as small, separate pull requests

## Data modelling & BI

- Dimensional modelling (Kimball): star and snowflake schemas, fact and dimension design, slowly changing dimensions (SCD types)
- ETL vs ELT pipeline design, data warehouse layering
- Applied end to end in [MusicaBI](https://github.com/LepsyMikolaj3301/MusicaBI): ingestion with dlt, orchestration in Airflow

## Engineering practices

**Containers & environments:** Docker, Docker Compose, devcontainers, multi-user Linux VMs<br>
**CI/CD:** GitLab CI, GitHub Actions<br>
**Code quality:** uv for dependency management, Ruff, MyPy, pre-commit hooks, pytest<br>
**Infra & networking:** Linux (Ubuntu), Tailscale, SSH tunnelling, self-hosted services

![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![GitLab CI](https://img.shields.io/badge/GitLab%20CI-FC6D26?style=for-the-badge&logo=gitlab&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/github%20actions-%232671E5.svg?style=for-the-badge&logo=githubactions&logoColor=white)
![uv](https://img.shields.io/badge/uv-DE5FE9?style=for-the-badge&logo=uv&logoColor=white)
![Ruff](https://img.shields.io/badge/Ruff-D7FF64?style=for-the-badge&logo=ruff&logoColor=black)
![pre-commit](https://img.shields.io/badge/pre--commit-FAB040?style=for-the-badge&logo=pre-commit&logoColor=black)
![Pytest](https://img.shields.io/badge/pytest-%23ffffff.svg?style=for-the-badge&logo=pytest&logoColor=2f9fe3)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Tailscale](https://img.shields.io/badge/Tailscale-242424?style=for-the-badge&logo=tailscale&logoColor=white)
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)

## Tech stack

**Data**<br>
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Apache Spark](https://img.shields.io/badge/Apache%20Spark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white)
![Apache Airflow](https://img.shields.io/badge/Airflow-017CEE?style=for-the-badge&logo=apacheairflow&logoColor=white)
![dlt](https://img.shields.io/badge/dlt-59C1D5?style=for-the-badge&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Polars](https://img.shields.io/badge/polars-CD792C?style=for-the-badge&logo=polars&logoColor=white)
![Postgres](https://img.shields.io/badge/postgres-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white)
![ArcadeDB](https://img.shields.io/badge/ArcadeDB-2C3E50?style=for-the-badge&logoColor=white)
![ArangoDB](https://img.shields.io/badge/ArangoDB-DDE072?style=for-the-badge&logoColor=black)

**ML / AI**<br>
![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-%230C55A5.svg?style=for-the-badge&logo=scipy&logoColor=white)
![Stable-Baselines3](https://img.shields.io/badge/Stable--Baselines3-2E7D32?style=for-the-badge&logoColor=white)

**Backend**<br>
![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi)

**Other**<br>
![C++](https://img.shields.io/badge/c++-%2300599C.svg?style=for-the-badge&logo=c%2B%2B&logoColor=white)


## GitHub stats

![GitHub metrics](https://raw.githubusercontent.com/LepsyMikolaj3301/LepsyMikolaj3301/main/metrics.svg)
