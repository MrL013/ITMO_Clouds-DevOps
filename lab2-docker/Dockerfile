FROM python:3.11.3

WORKDIR /usr/src/project

ENV AUTH_KEY = ${AUTH_KEY}

COPY requirements.txt . 

RUN apt-get update && \
    apt-get upgrade && \
    pip install -r --no-cache-dir requirements.txt

COPY . .

CMD ["user.py"] 
