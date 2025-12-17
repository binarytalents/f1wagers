# f1wagers — Formula 1 Friends Wager Platform

A private, invite-only Django platform for Formula 1 wagers with friends.

Built for fun, chaos, and long-running seasons: race-by-race wagers, chaos points,
and dynamic championship tables based on current standings — “What if the season ended today?”

## Features

- Race wagers (podium picks, fastest lap, chaos points)
- Season wagers (Driver & Constructor Champion – “What If?”)
- Separate Chaos Championship
- Admin-controlled current season
- Docker-based setup
- No public accounts
- No monetization
- Designed for private groups and friendly banter

## Requirements

- Docker
- Docker Compose


## Quick Start
cp .env.example .env
docker compose up --build -d
docker compose exec web python manage.py migrate
docker compose exec web python manage.py createsuperuser

Open in your browser:

- Web UI: http://localhost:10000
- Admin: http://localhost:10000/admin

## Project Structure

- f1data — Formula 1 seasons, races, and results
- wagers — Race wagers and season wagers
- webui — Frontend views and pages

## Rules

Wager rules and scoring details are available in:

docs/RULES.md

## Final Note

This platform exists for fun, friendly competition, and long-term bragging rights.

Any disputes will be resolved through sarcasm, screenshots,
and heated group chat discussions.
