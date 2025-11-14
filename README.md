### Anti-Corruption Cell
A unified Web, Mobile, and API platform for reporting, managing, and resolving public complaints. The system streamlines how citizens submit issues (e.g., road damage, drainage problems, garbage issues) and how administrators monitor, categorize, and solve them through integrated dashboards and mobile tools.

### Purpose of the Project
The objective of this project is to create a digital ecosystem that bridges communication between the public and authorities. It enables: 
* Easy submission of complaints via web or mobile app
* Status tracking for transparency 
* Efficient backend operations for administrators
* Real-time updates, notifications, and attachments
* A unified database that keeps complaint records organized.

This system reduces manual paperwork, speeds up responses, and ensures accountability in public service management.

### Key Features
For Citizens (Users)
* Create an account & login securely
* Submit complaints with category, location & photo attachments
* Track complaint status (Pending, Processing, Solved, Rejected)
* Comment on complaints
* Receive push & in-app notifications
* Access from both web and mobile app

For Admins
* Admin dashboard for full complaint overview
* Update complaint status & categories
* Manage users, feedback, comments
* View analytics: total complaints, solved, rejected, pending
* Auto-generated user performance metrics
* Review attachments submitted by users


### Technology Stack
* Frontend Web (acc-web)
* SvelteKit
* TailwindCSS
* Vite
* PostCSS
* REST API Integration
* Cookie-based authentication

Backend API (acc-backend)
* FastAPI
* SQLAlchemy ORM
* MySQL Database
* Pydantic Schemas
* Uvicorn
* Docker / Docker Compose
* Background Tasks & Notifications

Mobile App (acc-app)

* Flutter (Dart)
* Android & iOS support
* Provider / Riverpod (depending on your code)
* REST API integration
* Local storage (SharedPreferences or Hive)
* Network exception handling
* Material UI components


### Method 1: Run using Docker (Recommended & EASIEST)
* Step 1 — Install Docker: https://www.docker.com/products/docker-desktop/
* Step 2 — Open terminal inside your backend folder: cd acc-backend
* Step 3 — Run docker-compose: docker-compose up --build
* Step 4 — Open in browser


### Method 2: Run without Docker (Direct Python)
* Step 1 — Install Python: Use Python 3.10+
* Step 2 — Install Poetry: pip install poetry
* Step 3 — Install dependencies: cd acc-backend -> poetry install
* Step 4 — Activate virtual environment: poetry shell
* Step 5 — Run FastAPI server: uvicorn main:app --reload
* step 6 - Open your API


### Important Files 
(i) main.py → FastAPI entry point
(ii) pyproject.toml → dependencies
(iii) docker-compose.yml → backend + database
(iv) /config/db.py → database connection
(v) /scripts/*.sql → SQL data
(vi) /schemas/*.py → Pydantic models
(vii) /models/*.py → SQLAlchemy models
