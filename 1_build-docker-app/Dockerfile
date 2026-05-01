#use ECR public image for python 3.13 to avoid too many requests to Docker Hub
ARG REGISTRY="public.ecr.aws"
FROM  ${REGISTRY}/docker/library/python:3.13-slim

WORKDIR /src

COPY ./app/requirements.txt requirements.txt

RUN pip install --no-cache-dir -r requirements.txt

COPY ./app .

EXPOSE 5000

CMD ["python3", "app.py"]