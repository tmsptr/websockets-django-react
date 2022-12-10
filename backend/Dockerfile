FROM python:3.10-alpine

ENV PYTHONUNBUFFERED 1

EXPOSE 8000 8000

RUN apk update

WORKDIR /app/api

COPY requirements.txt ./

RUN pip install -r requirements.txt

COPY . ./

RUN ["/bin/sh"]