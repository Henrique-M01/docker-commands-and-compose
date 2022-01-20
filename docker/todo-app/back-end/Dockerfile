FROM node:16-alpine AS build
WORKDIR /app/back-end
COPY package*.json ./
RUN npm install
COPY . . 
EXPOSE 3001
CMD [ "npm" "start" ]