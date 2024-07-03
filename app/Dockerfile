# syntax=docker/dockerfile:1
FROM node:22-alpine
WORKDIR /app
COPY yarn.lock ./
COPY package.json ./
RUN yarn install --production
COPY . .
EXPOSE 3000
CMD ["node", "src/index.js"]
