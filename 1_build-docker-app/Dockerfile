FROM  python:3.13-slim

WORKDIR /src

COPY ./app/requirements.txt requirements.txt

RUN pip install --no-cache-dir -r requirements.txt

COPY ./app .

EXPOSE 5000

CMD ["python3", "app.py"]