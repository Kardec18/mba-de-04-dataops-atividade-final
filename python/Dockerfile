# NOTE name need to be Dockerfile
FROM python:3.9

ARG db_user
ARG db_password

ENV DB_USER $db_user
ENV DB_PASSWORD $db_password

RUN mkdir -p /usr/src/python/data/raw

WORKDIR /usr/src/python

COPY . /usr/src/python/

RUN pip install -r requirements.txt
