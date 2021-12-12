FROM node:lts-alpine
WORKDIR /app
COPY front/node_modules ./
COPY front/. ./
EXPOSE 8081
CMD ["yarn", "serve"]

