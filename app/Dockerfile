FROM python:3.7-buster

WORKDIR /app

RUN apt-get update && \
    apt-get install -y gdal-bin && \
    wget https://download.karrot.world/karrot-backend-production.pyz -O /app/karrot-backend.pyz

RUN sed -i -e's/ main/ main contrib non-free/g' /etc/apt/sources.list && \
    apt-get update && \
    apt-get install -y libmaxminddb0 libmaxminddb-dev geoipupdate

