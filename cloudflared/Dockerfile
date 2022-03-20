FROM visibilityspots/cloudflared

USER root

RUN apk update && apk add ca-certificates && rm -rf /var/cache/apk/* \
  mkdir /usr/local/share/ca-certificates/extra
COPY certs/mkcert.crt /usr/local/share/ca-certificates/extra
RUN update-ca-certificates
