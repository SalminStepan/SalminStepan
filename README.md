# Stepan Salmin

## Python Backend Developer

I build backend services, Telegram bots, data pipelines, and database-backed tools with Python.

My background is 11 years in the bar industry, so I like building software around real workflows: structured data, fast search, admin operations, clean input flows, and tools that people can actually use at work.

Right now I focus on Python backend development: FastAPI, PostgreSQL, aiogram, Pydantic, data parsing, and layered application architecture.

### Tech Stack

**Backend:** Python, FastAPI, aiogram  
**Databases:** PostgreSQL, SQL, psycopg  
**Data and validation:** Pydantic, JSON, JSON-LD, BeautifulSoup, httpx  
**Architecture:** handlers / services / repositories, CRUD, pagination, search, FSM, environment-based configuration  
**Tools:** Git, Linux, systemd, virtual environments

### What I Build

- Backend services with REST APIs, validation, repository layers, and PostgreSQL storage
- Telegram bots with real business scenarios, admin commands, FSM flows, and database-backed CRUD
- ETL/data preparation pipelines for collecting, extracting, normalizing, and saving structured data
- CLI tools with persistence, input validation, error handling, and clean separation of responsibilities

### Featured Projects

All projects below were built by me.

#### Cocktail Manager Bot

Telegram bot for managing a structured cocktail recipe database.

Built from scratch around a real bar workflow: adding recipes, searching cocktails, listing results with pagination, and managing admin-only operations.

**Highlights:**

- Full CRUD for cocktails and ingredients
- FSM-based step-by-step input flow
- Search by name and ingredients
- PostgreSQL schema for cocktails and structured ingredients
- Layered architecture: handlers, services, repositories, schemas
- Pydantic models for typed data validation
- Admin-only create, edit, and delete commands
- Deployed on a server with systemd

Repository: [cocktail_manager_bot_tg](https://github.com/SalminStepan/cocktail_manager_bot_tg)  
Live bot: [@Bartenders_Cocktail_bot](https://t.me/Bartenders_Cocktail_bot)

#### Cocktail ETL

Data pipeline for collecting and normalizing cocktail recipe data from structured web sources.

The pipeline reads sitemap URLs, downloads recipe pages, extracts JSON-LD Recipe data, stores raw data, normalizes recipe fields, and prepares clean JSON output for future import into a database or internal tool.

**Highlights:**

- Sitemap reader and recipe page fetcher
- JSON-LD Recipe extraction
- Raw and normalized JSON storage
- Ingredient normalization with parse status and parse errors
- Modular pipeline architecture
- Built as a Python package with `pyproject.toml`

Repository: [cocktail_etl](https://github.com/SalminStepan/cocktail_etl)

#### User Registry API

REST API for managing users with FastAPI and PostgreSQL.

**Highlights:**

- CRUD endpoints for user management
- Search and pagination
- PostgreSQL repository layer
- Pydantic request and response schemas
- Dependency injection for database access
- Swagger/OpenAPI documentation

Repository: [project_3_user_registry_API](https://github.com/SalminStepan/project_3_user_registry_API)

#### User Registry CLI with PostgreSQL

Command-line user registry backed by PostgreSQL.

**Highlights:**

- CRUD operations from the terminal
- Repository layer separated from CLI logic
- Parameterized SQL queries
- Case-insensitive search
- Domain-level error mapping
- Logging with configurable log level

Repository: [project_2_user_registry_pg](https://github.com/SalminStepan/project_2_user_registry_pg)

#### User Registry CLI

JSON-backed CLI application for managing users.

**Highlights:**

- Add, list, get, update, delete, and search commands
- JSON persistence
- Input validation and error handling
- Separation between command handling and storage logic

Repository: [user-registry-cli](https://github.com/SalminStepan/user-registry-cli)

### Engineering Focus

I care about code that is easy to read, easy to extend, and close to the problem it solves.

In my projects I practice:

- separating application layers instead of mixing database, business logic, and user interface code
- using PostgreSQL intentionally: schemas, constraints, indexes, parameterized queries
- designing practical CRUD flows with validation and predictable error handling
- turning domain knowledge into usable software, especially around bar operations and recipe data

### Contact

GitHub: [SalminStepan](https://github.com/SalminStepan)

Open to backend roles where I can work with Python, databases, APIs, bots, and practical business tools.
