FROM python:3.7-slim

RUN pip install flask prometheus_client

WORKDIR /home

COPY . .

CMD python app.py