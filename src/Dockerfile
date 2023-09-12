# syntax=docker/dockerfile:1
FROM python:3-alpine
ENV PYTHONUNBUFFERED=1
WORKDIR /usr/src/app
COPY requirements.txt /usr/src/app/
RUN pip install -U -r requirements.txt
COPY ./bot /usr/src/app/
ENTRYPOINT ["python", "main.py"]
