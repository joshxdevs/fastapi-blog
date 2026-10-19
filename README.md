# FastAPI Blog

A modern, hybrid web application and RESTful API built with **FastAPI**, **SQLAlchemy 2.0**, and **Jinja2** templates. It features server-side rendered pages with Bootstrap 5 (including custom themes and dark-mode support) alongside validated REST API endpoints with interactive OpenAPI documentation.

## Overview

`fastapi-blog` combines the speed and developer ergonomics of FastAPI with the flexibility of both server-side rendered (SSR) templates and a JSON REST API:

- **Frontend / SSR UI**: Responsive Bootstrap 5 interface with a dark/light/auto mode switcher, custom Google fonts (`Montserrat` and `Nunito`), and modular Jinja2 templates.
- **Backend / REST API**: Type-safe endpoints powered by Pydantic v2 schemas and SQLAlchemy 2.0 mapped models.
- **Smart Exception Handling**: Distinguishes between browser traffic (rendering styled HTML error pages) and API traffic (returning RFC-compliant JSON error details).


## Key Features

- **Dual-Mode Serving**: Browse posts via clean HTML views or integrate programmatically using `/api` JSON routes.
- **Interactive Documentation**: Instant Swagger UI (`/docs`) and ReDoc (`/redoc`) powered by OpenAPI.
- **ORM & Database Layer**: SQLite persistence via SQLAlchemy 2.0 declarative models with foreign key constraints and automatic schema creation.
- **Responsive Layout & Theming**: Bootstrap 5 with client-side theme switcher stored in `localStorage`.
- **Dynamic Asset Handling**: Static assets mounted at `/static` and user-uploaded content mounted at `/media`.
- **Fast Package Management**: Configured with `uv` and `pyproject.toml` for blazing fast environment management.
