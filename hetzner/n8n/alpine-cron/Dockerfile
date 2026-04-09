FROM alpine:3.21
RUN apk update && apk add docker curl aws-cli

COPY ./rootfs /

RUN chmod +x /usr/local/bin/ecr-login.sh
RUN chmod +x /usr/local/bin/entrypoint.sh

ENTRYPOINT [ "/usr/local/bin/entrypoint.sh" ]