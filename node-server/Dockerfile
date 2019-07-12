FROM node:11.15-alpine
ENV CHROME_BIN="/usr/bin/chromium-browser" \
  PUPPETEER_SKIP_CHROMIUM_DOWNLOAD="true"
RUN echo -e 'http://mirrors.aliyun.com/alpine/v3.9/main/\nhttp://mirrors.aliyun.com/alpine/v3.9/community/' > /etc/apk/repositories
RUN apk --no-cache update \ 
  && apk add supervisor ttf-freefont chromium \
  && npm install puppeteer@1.18.0 \
  &&  rm -fr /var/cache/apk/*