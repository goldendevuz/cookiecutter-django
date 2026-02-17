FROM python:3.12-slim-bookworm

ARG APP_HOME=/app
WORKDIR ${APP_HOME}

RUN apt-get update && apt-get install -y \
    build-essential \
    && rm -rf /var/lib/apt/lists/*

RUN pip install --no-cache-dir uv

CMD ["uv", "--help"]
