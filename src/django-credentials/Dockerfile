FROM python:3.10-slim

WORKDIR /app

COPY ../requirements.txt .

RUN pip install -r requirements.txt

COPY . .

RUN pip install gunicorn
RUN pip install psycopg2-binary

EXPOSE 9000
