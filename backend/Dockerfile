FROM python:alpine3.7

RUN apk add --no-cache \
    gcc \
    musl-dev \
    python3-dev \
    postgresql-dev

WORKDIR /code

COPY ./requirements.txt .
RUN pip install --upgrade pip wheel setuptools
RUN pip install -r requirements.txt

CMD ["./manage.py", "runserver", "0.0.0.0:8000"]
