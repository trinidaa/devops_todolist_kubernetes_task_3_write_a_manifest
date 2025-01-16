FROM python:3.12-slim

WORKDIR /app

COPY src/ /app/

RUN pip install --upgrade pip

RUN pip install -r requirements.txt

RUN python manage.py migrate

ENTRYPOINT ["python", "manage.py", "runserver", "0.0.0.0:8080"]