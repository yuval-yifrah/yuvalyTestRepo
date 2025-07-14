FROM python:latest

WORKDIR /src/app
COPY . /src/app/

ENV FLASK_APP=flaskr
ENV FLASK_ENV=development

RUN pip install --upgrade pip
RUN pip install -e .

RUN flask init-db

EXPOSE 5000
CMD ["flask","run","--host=0.0.0.0"]
