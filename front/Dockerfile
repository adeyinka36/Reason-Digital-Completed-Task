FROM node:lts-alpine
WORKDIR /app
COPY package*.json ./
COPY . ./
RUN rm -rf node_modules package.lock.json yarn.lock
RUN yarn install && yarn
RUN npm i -g @vue/cli-service
RUN npm i -g @vue/cli-plugin-babel
RUN npm i -g @vue/cli-plugin-eslint
RUN npm i -g @vue/cli-plugin-router
RUN npm i -g @vue/cli-plugin-vuex
RUN npm i -g @vue/compiler-sfc
EXPOSE 8081
CMD ["yarn", "serve"]