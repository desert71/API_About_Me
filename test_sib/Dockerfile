FROM python:3.12
COPY . .
WORKDIR .
RUN pip install poetry && poetry config virtualenvs.in-project true && poetry run new && poetry run install
EXPOSE 8000
CMD ["uvicorn", "simple:app", "--host", "127.0.0.1"]