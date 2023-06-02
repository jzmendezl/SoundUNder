FROM nginx

COPY /SoundUNder_ag_rp/app.conf /etc/nginx/conf.d/default.conf

COPY /certs/34_27_78_242.crt /etc/ssl/certs/
COPY /certs/34_27_78_242.key /etc/ssl/private/

RUN mkdir /etc/log