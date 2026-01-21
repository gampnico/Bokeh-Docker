FROM alpine:3

RUN apk add --update --no-cache docker-cli docker-cli-compose docker-cli-buildx git bash

ENV \
	WS_ORIGIN=bokeh.oggm.org

COPY run.sh /root/run.sh
COPY repo/ /root/repo/
# COPY ../../../dtcg-web-docker/ /root/repo/dtcg-web/

WORKDIR /root
ENTRYPOINT ["/root/run.sh"]
