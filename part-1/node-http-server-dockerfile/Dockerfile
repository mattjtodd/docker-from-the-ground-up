FROM alpine:3.8

RUN apk add --no-cache npm

RUN npm install http-server -g

WORKDIR /etc/files

COPY greeting.txt ./

RUN chown nobody:nobody *

USER nobody

CMD ["http-server", "./"]