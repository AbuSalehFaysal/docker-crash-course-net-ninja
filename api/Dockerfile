FROM node:16-alpine

RUN npm install -g nodemon

WORKDIR /app

COPY package.json .

COPY . .

RUN npm install

EXPOSE 4000

# The below instruction will be executed when a Docker Container Starts
CMD ["npm", "run", "dev"]