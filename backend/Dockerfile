FROM python:3.11.12-slim

COPY requirements.txt requirements.txt
RUN cat /etc/resolv.conf # Add this line to see the DNS config
RUN pip install -r requirements.txt

COPY . .

CMD [ "python", "main.py" ]