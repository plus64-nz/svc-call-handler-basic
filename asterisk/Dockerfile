FROM alpine:3.10
LABEL maintainer="Michael Walton"
WORKDIR /root/

RUN apk update \
  && apk add asterisk asterisk-sample-config asterisk-sounds-en

COPY etc /etc/

EXPOSE 5060 5061
CMD ["asterisk","-vvv","-f"]