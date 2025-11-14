





## Method 1: Run using Docker (Recommended & EASIEST)
Step 1 — Install Docker: https://www.docker.com/products/docker-desktop/
Step 2 — Open terminal inside your backend folder: cd acc-backend
Step 3 — Run docker-compose: docker-compose up --build
Step 4 — Open in browser


## Method 2: Run without Docker (Direct Python)
Step 1 — Install Python: Use Python 3.10+
Step 2 — Install Poetry: pip install poetry
Step 3 — Install dependencies: cd acc-backend -> poetry install
Step 4 — Activate virtual environment: poetry shell
Step 5 — Run FastAPI server: uvicorn main:app --reload
step 6 - Open your API


## Important Files 
main.py → FastAPI entry point
pyproject.toml → dependencies
docker-compose.yml → backend + database
/config/db.py → database connection
/scripts/*.sql → SQL data
/schemas/*.py → Pydantic models
/models/*.py → SQLAlchemy models
