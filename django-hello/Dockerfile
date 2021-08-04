FROM python:3.8-alpine
#FROM python:3.9
ENV PYTHONUNBUFFERED 1

#RUN mkdir /app
WORKDIR /app

COPY ./kubeBert/ /app/
COPY requirements.txt /app/requirements.txt
RUN pip install -r requirements.txt

#COPY . /app

#EXPOSE 8000

CMD [ "python3", "manage.py", "runserver", "0.0.0.0:8000" ]

#CMD python manage.py runserver 0.0.0.0:8000