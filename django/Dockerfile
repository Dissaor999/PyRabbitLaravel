FROM python:3.10
RUN apt-get update \
    && apt-get install -y --no-install-recommends
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1
WORKDIR /app
COPY requiere.txt /app/requiere.txt
RUN pip install --upgrade pip && pip install -r requiere.txt
COPY . /app