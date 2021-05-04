FROM python:3.9.4

RUN pip install psycopg2 djangorestframework django-cors-headers pylint coverage

WORKDIR /backend

COPY . .

CMD python3 manage.py migrate && python3 manage.py runserver 0.0.0.0:8000
