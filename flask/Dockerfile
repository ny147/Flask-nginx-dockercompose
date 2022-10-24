from python:3.9

WORKDIR /flask

COPY . .

RUN apt-get update
RUN apt install libsndfile1 -y
RUN pip install -r requirement.txt

CMD gunicorn --bind 0.0.0.0:5000 run:app