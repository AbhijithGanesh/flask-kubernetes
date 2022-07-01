FROM python:3.9-slim

COPY requirements.txt base.txt
COPY . /app

RUN ["python", "-m", "pip", "install", "-U", "pip"]
RUN ["pip", "install", "-r", "base.txt"]

WORKDIR  /app

CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0", "-p","8000", "--no-debugger"]

EXPOSE 8000:8000
