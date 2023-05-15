FROM python:3
RUN apt-get update && apt-get install python3-pip -y && pip3 install flask && pip3 install psycopg2 && pip3 install configparser
WORKDIR /srv/app/
CMD ["python", "web.py"]
