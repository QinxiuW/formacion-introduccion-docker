FROM node:14.0.0
ENV HOST 0.0.0.0
COPY ./ /app
WORKDIR /app
RUN NODE_ENV=build npm install

EXPOSE 3000
RUN yarn install && yarn build

CMD [ "node", "node_modules/nuxt/bin/nuxt.js" ]
