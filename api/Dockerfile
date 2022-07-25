FROM node:17-alpine

WORKDIR /app

COPY . .

RUN npm install

EXPOSE 4000

# The below instruction will be executed when a Docker Container Starts
CMD ["node", "app.js"]