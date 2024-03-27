FROM python:3.12

EXPOSE 80/tcp

WORKDIR /src

COPY . .

RUN pip3 install -r requirements.txt

CMD ["python3.12", "-m", "flask", "run", "--host=0.0.0.0", "--port=80"]
