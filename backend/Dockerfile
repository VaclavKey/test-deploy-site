FROM python:3.11.12-slim

RUN ping -c 4 google.com

COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt

COPY . .

CMD [ "python", "main.py" ]