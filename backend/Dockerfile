FROM python:3.11.12-slim

RUN echo "nameserver 8.8.8.8" > /etc/resolv.conf

RUN apt-get update && apt-get install -y iputils-ping dnsutils

COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt

COPY . .

CMD [ "python", "main.py" ]