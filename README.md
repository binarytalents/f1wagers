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
~~~  bash
cp .env.example .env
cker compose up --build -d
docker compose exec web python manage.py migrate
docker compose exec webdocker compose exec web python manage.py createsuperuser
~~~
Web UI: http://localhost:10000 Admin: http://localhost:10000/admin

## Project Structure

- f1data — Formula 1 seasons, races, and results
- wagers — Race wagers and season wagers
- webui — Frontend views and pages

## Rules & Scoring

Before playing, make sure to read the full rules and scoring system:

[F1 Pick Champions — Rules & Scoring](docs/RULES.md)

This document explains:
- How wagers work
- Podium and Joker rules
- Chaos points and Chaos Championship
- Scoring system and championships

## Disclaimer & Copyright

This project is an unofficial, fan-made application.

Formula 1, F1, FIA, Formula One World Championship, and related trademarks are the
property of their respective owners. This project is not affiliated with, endorsed by,
or connected to Formula 1, the FIA, or any associated organizations.

All team names, driver names, race names, and results are used strictly for
informational and recreational purposes.

No commercial use is intended.

## License

This project is released under the MIT License.

You are free to use, modify, and distribute this software, provided that the original
copyright notice and this permission notice are included in all copies or substantial
portions of the software.

See the LICENSE file for full license text.

## Final Note

This platform exists for fun, friendly competition, and long-term bragging rights.

Any disputes will be resolved through sarcasm, screenshots,
and heated group chat discussions.
