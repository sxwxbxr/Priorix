# Priorix
Ein Task Priorisierer mit KI der Wichtigkeit Aufwand Risiko und Deadline bewertet.

## Ziel
Tagesfokus Vorschlaege basierend auf Regeln und LLM Scoring.

## Features
* Aufgaben Import aus Todoist GitHub Issues CSV
* Scoring Matrix mit Gewichtungen
* Tagesplan Generator
* Erklaerbare Vorschlaege mit Faktoren

## Tech Stack
* Python FastAPI
* React Next.js
* SQLite oder Postgres
* Optional lokales LLM ueber llama cpp python

## Kritische Packages
* fastapi pydantic
* scikit learn optional
* numpy pandas
* llama cpp python optional
* zod react query
* next auth bei Multi User

## Env Variablen
* MODEL_PATH optional
* OPENAI_API_KEY optional falls Cloud LLM

## API
* POST tasks import
* POST tasks score
* GET plan today

## Datenmodell
* task title desc deadline effort impact risk source

## Setup
* make dev startet api und web

## Tests
* Deterministische Scores bei fixen Gewichten

## CI
* Mypy Ruff Pytest
* Web Lint Test Build

## Security
* Lokale Verarbeitung wenn moeglich

## Roadmap
* Kalender Blocker
* Team Sharing

## Lizenz
MIT
