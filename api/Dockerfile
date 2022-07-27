FROM node:16-alpine

WORKDIR /app

COPY package.json .

COPY . .

RUN npm install

EXPOSE 4000

# The below instruction will be executed when a Docker Container Starts
CMD ["node", "app.js"]