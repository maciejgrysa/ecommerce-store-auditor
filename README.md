> **Portfolio showcase** — the complete implementation is kept private to protect intellectual property. This public repository intentionally contains documentation only. A live demo or private code review can be provided for a serious project discussion.

# Ecommerce Store Auditor

FastAPI application that checks publicly visible ecommerce issues and generates a structured audit report.

## Checks
- missing product price, image, brand or EAN
- structured-data availability
- GPSR-related manufacturer information
- Omnibus promotion-price signals
- sitemap availability
- SSL expiry
- product-feed vs website inconsistencies
- unreachable product pages and technical failures

## Engineering highlights
- async crawling with strict concurrency and response-size limits
- URL/host safety restrictions
- SQLite task queue with WAL and cleanup/retention
- per-IP rate limiting
- background scan lifecycle and restart recovery
- healthcheck and security headers
- secret scanning and release checks

## Stack
Python 3.13, FastAPI, httpx, lxml, Jinja2, SQLite, pytest.

Designed for public data only and intentionally limits request volume.

## Usage and licensing

This repository is source-available for portfolio evaluation. You may inspect the code and run an unmodified local copy for evaluation, but commercial use, redistribution, republishing and derivative distribution are not permitted without written permission. See [LICENSE.md](LICENSE.md).

