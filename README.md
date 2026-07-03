# Stepan Salmin

Junior Python Backend Developer

I build backend services, Telegram bots, data pipelines, and PostgreSQL-backed tools with Python.

My current work is mostly around structured cocktail data: collecting recipes, normalizing ingredients, storing them in PostgreSQL, and making them searchable through bots and backend services.

Before moving into software development, I spent 11 years in the bar industry. That background helps me build projects around real workflows instead of abstract examples.

## Tech Stack

**Backend:** Python, FastAPI, aiogram  
**Databases:** PostgreSQL, SQL, psycopg  
**Data:** JSON, JSON-LD, XML, httpx, BeautifulSoup  
**Validation and testing:** Pydantic, pytest  
**Architecture:** handlers, services, repositories, CRUD, pagination, FSM, environment-based configuration  
**Tools:** Git, Linux, systemd, virtual environments

## Projects

### Cocktail ETL

[cocktail_etl](https://github.com/SalminStepan/cocktail_etl)

ETL pipeline for collecting, extracting, normalizing, and importing cocktail recipes from Difford's Guide into PostgreSQL.

Pipeline:

```text
sitemap.xml -> recipe URLs -> HTML pages -> JSON-LD Recipe -> raw JSON -> clean JSON -> PostgreSQL
```

Current full scrape results:

* 6,892 recipe URLs found
* 6,614 raw recipes extracted
* 6,614 clean recipes generated
* 6,614 cocktails loaded into PostgreSQL
* 30,761 ingredients stored
* 0 failed recipes
* about 96.0% extraction coverage
* about 84.9% fully normalized recipes
* about 99.88% ingredient parse coverage

What it includes:

* sitemap XML parsing;
* delayed page fetching with `httpx`;
* JSON-LD `Recipe` extraction from HTML;
* recipe normalization for ingredients, method, glass, garnish, description, and image URL;
* parse quality tracking through `parse_status` and `parse_errors`;
* idempotent PostgreSQL import using `source_url`;
* ingredient replacement on re-import to avoid duplicates;
* pytest coverage for normalization logic.

Stack: Python, PostgreSQL, psycopg, httpx, BeautifulSoup, JSON-LD, XML, pytest.

### Cocktail Manager Bot

[cocktail_manager_bot_tg](https://github.com/SalminStepan/cocktail_manager_bot_tg)  
Live bot: [@Bartenders_Cocktail_bot](https://t.me/Bartenders_Cocktail_bot)

Telegram bot for managing a cocktail recipe database.

What it includes:

* CRUD operations for cocktails and ingredients;
* PostgreSQL storage;
* search by cocktail name and ingredients;
* paginated cocktail list;
* full recipe view;
* FSM-based recipe creation and editing flow;
* admin-only create, edit, and delete commands;
* Pydantic schemas;
* layered structure: handlers, services, repositories, schemas, database;
* parameterized SQL queries and whitelist-based field updates.

Stack: Python, aiogram, PostgreSQL, psycopg, Pydantic, pytest.

### User Registry API

[project_3_user_registry_API](https://github.com/SalminStepan/project_3_user_registry_API)

REST API for user management with FastAPI and PostgreSQL.

Includes CRUD endpoints, search, pagination, partial updates, Pydantic schemas, repository layer, dependency-based database access, and Swagger/OpenAPI documentation.

Stack: Python, FastAPI, PostgreSQL, psycopg, Pydantic, Uvicorn.

### User Registry CLI with PostgreSQL

[project_2_user_registry_pg](https://github.com/SalminStepan/project_2_user_registry_pg)

Command-line user registry backed by PostgreSQL.

Includes terminal CRUD commands, repository layer, parameterized SQL queries, case-insensitive search with `ILIKE`, error handling, logging, and environment-based configuration.

Stack: Python, PostgreSQL, psycopg, SQL, logging.

### User Registry CLI

[user-registry-cli](https://github.com/SalminStepan/user-registry-cli)

JSON-backed CLI application for user management.

Includes add, list, get, update, delete, and search commands, JSON persistence, input validation, and separation between command logic and storage logic.

## Current Focus

* Building a stronger FastAPI backend around the cocktail database;
* adding SQLAlchemy and Alembic to future backend projects;
* improving Docker, API tests, CI, and production-style project setup;
* keeping the cocktail ETL and bot connected to practical use cases.

## Contact

GitHub: [SalminStepan](https://github.com/SalminStepan)

Open to junior Python backend roles involving APIs, PostgreSQL, Telegram bots, ETL pipelines, and internal business tools.
