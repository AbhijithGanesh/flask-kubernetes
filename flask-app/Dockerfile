FROM python:3.9-slim

COPY requirements.txt base.txt
COPY . /app

RUN ["python", "-m", "pip", "install", "-U", "pip"]
RUN ["pip", "install", "-r", "base.txt"]

WORKDIR  /app


