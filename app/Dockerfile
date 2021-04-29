 # syntax=docker/dockerfile:1
 ARG FOO="default"
 FROM node:12-alpine
 ARG FOO
 RUN echo $FOO
 RUN apk add --no-cache python g++ make
 WORKDIR /app
 COPY . .
 RUN yarn install --production
 CMD ["node", "src/index.js"]