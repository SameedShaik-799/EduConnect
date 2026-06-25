# Parent Edu Connect

Full-stack AI student monitoring system: **Java Spring Boot + MySQL + Python + HTML/JS**.

## Quick Start

1. **MySQL Workbench** — connect as `root` / `7993445360`
2. Run `database/schema.sql` then `database/seed.sql` (optional; backend auto-seeds on first run)
3. Double-click **`start-all.bat`** OR run manually:

```bash
cd python-ai && pip install -r requirements.txt && python app.py
cd backend && mvn spring-boot:run
# Open index.html in browser
```

## Demo Logins

| Role | Email | Password |
|------|-------|----------|
| Parent | parent@demo.edu | parent123 |
| Teacher | teacher@demo.edu | teacher123 |
| Admin | admin@demo.edu | admin123 |

## Project Structure

```
index.html, app.js, styles.css     → Frontend (calls API on port 8080)
backend/                           → Java Spring Boot REST API
python-ai/                         → Python Flask AI service (port 5000)
database/schema.sql, seed.sql      → MySQL Workbench scripts
docs/PROJECT_DOCUMENTATION.pdf       → Full technical report
SETUP.md                           → Detailed setup guide
```

## Documentation

- **PDF Report:** `docs/PROJECT_DOCUMENTATION.pdf`
- **Setup Guide:** `SETUP.md`

## Note

If `mvn` fails due to OneDrive path encoding, build from an ASCII path:

```powershell
Copy-Item -Recurse backend C:\temp\parent-edu-build
cd C:\temp\parent-edu-build
mvn spring-boot:run
```
