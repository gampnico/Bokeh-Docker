FROM alpine:3

RUN apk add --update --no-cache docker-cli docker-cli-compose git bash vim

ENV \
	WS_ORIGIN=localhost

COPY run.sh /root/run.sh
WORKDIR /root
ENTRYPOINT ["/root/run.sh"]
