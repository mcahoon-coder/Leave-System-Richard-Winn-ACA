Render Quick Deploy:

Build Command:
  pip install -r requirements.txt

Start Command:
  gunicorn -w 2 -k gthread -b 0.0.0.0:$PORT app:app

Env Vars:
  SECRET_KEY=ChangeThisSecret123!
  (Optional) DATABASE_URL=postgresql://user:pass@host:5432/dbname
