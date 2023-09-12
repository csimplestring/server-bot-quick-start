# syntax=docker/dockerfile:1
FROM python:3.10.13-bookworm
ENV PYTHONUNBUFFERED=1
WORKDIR /usr/src/app
COPY requirements.txt /usr/src/app/
RUN pip install -U -r requirements.txt
COPY ./bot /usr/src/app/
CMD ["uvicorn", "main:fastapi_app", "--host", "0.0.0.0", "--port", "5000"]
