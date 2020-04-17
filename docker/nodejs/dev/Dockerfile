FROM node:13.13.0-alpine3.10

RUN mkdir -p /usr/src/app

WORKDIR /usr/src/app

COPY ./ ./

# Set the container entrypoint
COPY ./docker/nodejs/dev/entrypoint.sh /
RUN chmod 755 /entrypoint.sh
RUN chmod +x /entrypoint.sh

ENTRYPOINT ["/entrypoint.sh"]

CMD ["/entrypoint.sh"]