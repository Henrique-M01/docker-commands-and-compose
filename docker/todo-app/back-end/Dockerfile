FROM node:16-alpine AS build
WORKDIR /app/back-end
COPY package*.json ./
ADD node_modules.tar.gz ./todo-app/back-end
RUN npm install
COPY . . 
EXPOSE 3001
CMD [ "npm" "start" ]