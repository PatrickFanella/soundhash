# SoundHash

SoundHash is a Python application for identifying short audio clips by fingerprinting video audio and matching it against previously ingested YouTube content. I built it to demonstrate the kind of backend and data-engineering work I enjoy most: turning messy media inputs into a reliable, searchable system.

## Why it stands out

- Designed an end-to-end ingestion and processing pipeline for YouTube audio
- Applied digital signal processing techniques to generate compact audio fingerprints
- Built backend services with Python, FastAPI, SQLAlchemy, and PostgreSQL
- Structured the project for real-world operation with Docker, environment-based config, logging, and background job tracking
- Added automated testing, linting, type checking, and CI workflows to support maintainability

## Technical highlights

- **Backend engineering:** Python 3, FastAPI, SQLAlchemy, Alembic
- **Data & storage:** PostgreSQL, repository pattern, processing job lifecycle management
- **Media processing:** `yt-dlp`, `ffmpeg`, spectral analysis, fingerprint hashing
- **Platform/API work:** YouTube integration, OAuth flows, REST endpoints, auth and rate limiting
- **Developer experience:** pytest, Ruff, Black, mypy, Docker, GitHub Actions

## What this project demonstrates

This project showcases my ability to:

- design and ship multi-stage processing pipelines
- work across APIs, databases, and media-processing tools
- translate technical complexity into maintainable application architecture
- build software with production-minded practices rather than one-off scripts

## Quick look

```bash
python scripts/setup_database.py
python scripts/ingest_channels.py --dry-run --max-videos 5
```

## Repository structure

- `src/core/` – audio fingerprinting and video processing
- `src/ingestion/` – orchestration for channel ingestion and processing jobs
- `src/database/` – database models, connections, and repositories
- `src/api/` – YouTube integration and API-related services
- `config/` – centralized settings and logging configuration

## Notes for reviewers

If you're evaluating this project as part of a job application, the main strengths to look for are system design, backend implementation, data pipeline thinking, and practical use of Python tooling around a non-trivial media problem.
