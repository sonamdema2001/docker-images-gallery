# FROM python:3.10.7

# WORKDIR /app

# EXPOSE 5050

# COPY Pipfile Pipfile.lock ./

# RUN pip install pipenv

# RUN pipenv lock
# RUN pipenv run pip freeze > requirements.txt

# COPY . ./

# CMD ["python", "main.py"]


FROM python:3.10.7

WORKDIR /app

COPY . ./

# Install dependencies manually
RUN pip install --no-cache-dir \
    requests \
    flask \
    python-dotenv \
    flask-cors

CMD ["python", "main.py"]
