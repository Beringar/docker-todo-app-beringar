FROM node:18-alpine
LABEL org.opencontainers.image.source https://github.com/Beringar/docker-todo-app-beringar
WORKDIR /app
COPY package.json yarn.lock ./
RUN yarn install --production
COPY . .
CMD ["node", "src/index.js"]
