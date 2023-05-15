FROM python:3.7.2-alpine3.8
RUN apk --update-cache upgrade && apk add --no-cache postgresql-dev && apk add --no-cache py3-pip && apk add --no-cache libpq && apk add --virtual .build-deps gcc python-dev musl-dev && pip install flask && pip install psycopg2-binary && pip install psycopg2 && pip install configparser
WORKDIR /srv/app/
CMD ["python", "web.py"]
