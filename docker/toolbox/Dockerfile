FROM node:12.16.2-alpine3.11
RUN apk --no-cache --update --virtual build-dependencies add \
    python \
    make \
    g++
WORKDIR /app
COPY . .
RUN npm ci
RUN npm run build --prod