FROM python:latest

WORKDIR /app

COPY . /app

RUN pip install --no-cache-dir -r requirements.txt

ENV FLASK_APP=app.py


CMD [ "python3","-m","flask","run","--host=0.0.0.0","--port=80"]