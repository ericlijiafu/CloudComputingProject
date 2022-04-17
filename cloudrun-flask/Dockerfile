#e the official lightweight Python image.
# https://hub.docker.com/_/python
FROM python:3.9-slim

FROM public.ecr.aws/lambda/python:3.8

RUN mkdir -p /app
COPY . main.py /app/
WORKDIR /app
RUN pip install -r requirements.txt
EXPOSE 8080
CMD [ "main.py" ]
ENTRYPOINT [ "python" ]
