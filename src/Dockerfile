FROM node:alpine
LABEL maintaner="ronjericsantos.gss@gmail.com"
USER root:root
COPY . /usr/src/app
WORKDIR /usr/src/app
ENV PATH /usr/src/app/node_modules/.bin:$PATH
RUN apk update && apk add yarn \
    npm \
    bash \
    && rm /var/cache/apk/*
CMD ["npm", "start"]