FROM python:3.8

WORKDIR /app

COPY ./pyproject.toml .
COPY ./poetry.lock .

RUN pip install poetry
RUN poetry config virtualenvs.create false
RUN poetry install --no-ansi --no-dev --no-interaction

COPY . .
