FROM python:3.11

EXPOSE 80/tcp

WORKDIR /src

COPY . .

RUN pip3.11 install -r requirements.txt

CMD ["python3.11", "-m", "flask", "run", "--host=0.0.0.0", "--port=80"]
