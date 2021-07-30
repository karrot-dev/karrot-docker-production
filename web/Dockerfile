FROM nginx:stable

RUN apt-get update && \
    apt-get install -y unzip && \
    curl https://download.karrot.world/karrot-frontend-production.zip -o karrot-frontend.zip && \
    unzip -o karrot-frontend.zip -d /usr/share/nginx/html

COPY ./nginx.conf /etc/nginx/conf.d/default.conf