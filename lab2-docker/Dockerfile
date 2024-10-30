FROM python:3.11.3

WORKDIR /usr/src/project

ENV AUTH_KEY = ${AUTH_KEY}

COPY requirements.txt . 

RUN apt-get update && \
    apt-get upgrade -y && \
    pip install --no-cache-dir -r requirements.txt

COPY . .

CMD ["python", "user.py"] 
