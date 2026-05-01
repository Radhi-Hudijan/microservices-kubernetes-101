# Use ECR public image for Python 3.10
FROM public.ecr.aws/docker/library/python:3.10-slim     

WORKDIR /src

COPY ./app/requirements.txt requirements.txt

RUN pip install --no-cache-dir -r requirements.txt

COPY ./app .

EXPOSE 5000

CMD ["python3", "app.py"]