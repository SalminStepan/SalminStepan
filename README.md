# Stepan Salmin

## Python Backend Developer

Python backend developer focused on backend services, Telegram bots, data pipelines, and PostgreSQL-backed applications.

Main stack: Python, FastAPI, PostgreSQL, aiogram, Pydantic, psycopg, SQL, JSON/JSON-LD, httpx, BeautifulSoup, Git, Linux.

Background: 11 years in the bar industry. Current projects are mostly related to structured recipe data, internal tools, CRUD workflows, search, and automation.

## Tech Stack

**Backend:** Python, FastAPI, aiogram
**Databases:** PostgreSQL, SQL, psycopg
**Data:** JSON, JSON-LD, BeautifulSoup, httpx
**Validation:** Pydantic
**Architecture:** handlers, services, repositories, CRUD, pagination, FSM, environment-based configuration
**Tools:** Git, Linux, systemd, virtual environments, pytest

## Projects

### Cocktail Manager Bot

Telegram bot for managing a cocktail recipe database.

Features:

* CRUD for cocktails and ingredients
* PostgreSQL storage
* Search by cocktail name and ingredients
* Paginated cocktail list
* FSM-based recipe creation flow
* Admin-only create, edit, and delete commands
* Pydantic schemas
* Layered structure: handlers, services, repositories
* Server deployment with systemd

Repository: [cocktail_manager_bot_tg](https://github.com/SalminStepan/cocktail_manager_bot_tg)
Live bot: [@Bartenders_Cocktail_bot](https://t.me/Bartenders_Cocktail_bot)

### Cocktail ETL

ETL pipeline for collecting, extracting, normalizing, and importing cocktail recipe data.

Features:

* Sitemap URL extraction
* Recipe page fetching
* JSON-LD `Recipe` extraction
* Raw JSON storage
* Clean normalized JSON output
* Ingredient parsing
* Parse status and parse error tracking
* PostgreSQL schema
* Idempotent cocktail upsert by `source_url`
* Ingredient replacement on re-import
* CLI command for importing clean JSON into PostgreSQL
* Pytest coverage for normalization logic

Repository: [cocktail_etl](https://github.com/SalminStepan/cocktail_etl)

### User Registry API

REST API for user management with FastAPI and PostgreSQL.

Features:

* CRUD endpoints
* Search and pagination
* PostgreSQL repository layer
* Pydantic request and response schemas
* Dependency-based database access
* Swagger/OpenAPI documentation

Repository: [project_3_user_registry_API](https://github.com/SalminStepan/project_3_user_registry_API)

### User Registry CLI with PostgreSQL

Command-line user registry backed by PostgreSQL.

Features:

* CRUD operations from terminal
* Repository layer separated from CLI logic
* Parameterized SQL queries
* Case-insensitive search
* Error handling
* Logging

Repository: [project_2_user_registry_pg](https://github.com/SalminStepan/project_2_user_registry_pg)

### User Registry CLI

JSON-backed CLI application for user management.

Features:

* Add, list, get, update, delete, and search commands
* JSON persistence
* Input validation
* Error handling
* Separation between command logic and storage logic

Repository: [user-registry-cli](https://github.com/SalminStepan/user-registry-cli)

## Current Focus

* Python backend development
* FastAPI
* PostgreSQL
* Telegram bots
* ETL/data preparation
* Testing with pytest
* Clean project structure and layered architecture

## Contact

GitHub: [SalminStepan](https://github.com/SalminStepan)

Open to junior Python backend roles involving APIs, databases, bots, ETL pipelines, and internal business tools.
