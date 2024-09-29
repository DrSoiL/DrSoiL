# Substrate Optimization

## Voraussetzungen
- Docker
- Docker Compose

## Installation und Ausführung

1. Klone das Repository:
    ```bash
    git clone <repository-url>
    cd substrate-optimization
    ```

2. Starte Docker Compose:
    ```bash
    docker-compose up --build
    ```

3. Die API ist unter `http://localhost:8000` verfügbar und die Frontend-Anwendung unter `http://localhost:3000`.

## Umgebungsvariablen
Erstelle eine `.env`-Datei mit den folgenden Werten:
```bash
DATABASE_URL="postgresql://user:password@db/substrate_db"
# Substrate Optimization System

## Overview

This system provides an interface for optimizing substrate mixtures for plant growth by taking into account different nutrients, microorganisms, flavonoids, humic acids, phytohormones, and other beneficial compounds. It uses a FastAPI backend, PostgreSQL for data storage, and a React.js frontend for user interaction.

## Key Components

1. **Backend**: FastAPI for API development, SQLAlchemy for ORM, PostgreSQL for database management.
2. **Frontend**: React.js for a dynamic and responsive user interface.
3. **Optimization**: Uses DEAP for multi-objective optimization (NSGA-II algorithm).
4. **Containerization**: Docker and Docker Compose for environment consistency.

## Installation Instructions

### Prerequisites

Ensure you have Docker and Docker Compose installed.

### Setup

1. Clone the repository:
    ```bash
    git clone https://github.com/your-repo/substrate-optimization.git
    cd substrate-optimization
    ```

2. Create a `.env` file in the root directory with the following content:

    ```bash
    DATABASE_URL=postgresql://user:password@db/substrate_db
    ```

3. Build and start the containers using Docker Compose:

    ```bash
    docker-compose up --build
    ```

4. Access the application:
    - Backend API: [http://localhost:8000](http://localhost:8000)
    - Frontend: [http://localhost:3000](http://localhost:3000)

## Usage

- **Create a product**: Input detailed data about the strain, nutrients, and other properties.
- **Create a mixture**: Generate an optimized mixture based on the nutrient needs of plants.
- **Multi-objective optimization**: Run the optimization algorithm to get the best substrate mixtures.

