## Backend Architecture (Modular Monolith)
The backend is organized as a modular monolith with a single entrypoint and clear separation of responsibilities. Each module focuses on one concern so teams can develop features in parallel.

## Core Capabilities
- Authentication and session management
- Machine, system, and configuration APIs
- Server-side rendering for web pages
- Integration points for email notifications
- Centralized configuration and environment checks

## Module Overview
- App composition and startup wiring
- Core configuration, database setup, and runtime state
- ORM models for persistent entities
- Service layer for security and notifications
- Router layer for API and web endpoints

## Extension Rules (High-Level)
- New data tables belong in the models layer
- New business logic belongs in services
- New endpoint groups belong in routers
- New config or env keys belong in core config

## Tech Stack (Backend)
- Python
- FastAPI-style routing with HTML template support
- SQLAlchemy ORM
- Gunicorn for production entrypoint

## Operational Notes
- Stable entrypoint with isolated app wiring
- Structure supports unit testing by layer
- Designed for incremental growth (schemas, migrations, repositories)

## Notes for Reviewers
- This README is intentionally high-level to avoid sharing proprietary code.
- Detailed code walkthroughs can be shared in a private session if needed.

## Contact
If you would like a guided walkthrough, architecture notes, or a feature demo, please reach out www.mectosys.com.
