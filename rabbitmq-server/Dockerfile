FROM rabbitmq:3.7-management-alpine

RUN echo -e 'http://mirrors.aliyun.com/alpine/v3.8/main/\nhttp://mirrors.aliyun.com/alpine/v3.8/community/' > /etc/apk/repositories

RUN apk add --update --no-cache vim  tzdata