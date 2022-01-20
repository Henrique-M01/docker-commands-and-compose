FROM node:16-alpine AS build

WORKDIR /app/front-end

COPY package*.json ./

ADD node_modules.tar.gz ./todo-app/front-end

RUN npm install

COPY . . 

EXPOSE 3000

CMD [ "npm" "start" ]
