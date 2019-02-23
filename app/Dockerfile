FROM python:3.6-alpine
RUN mkdir /var/www
WORKDIR /var/www
EXPOSE 3031
COPY requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt
WORKDIR /var/www/src
CMD ["uwsgi","--ini","/var/www/uwsgi.ini"]