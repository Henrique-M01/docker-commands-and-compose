FROM node:14-alpine AS build
WORKDIR /app/front-end
COPY package*.json ./
RUN npm install
ADD node_modules.tar.gz ./docker/todo-app/front-end
COPY . . 
RUN npm run build

FROM nginx:1.16.0-alpine AS prod
COPY ./docker/todo-app/front-end /usr/share/nginx/html
EXPOSE 3001
ENTRYPOINT ["nginx", "-g", "daemon off;"]
CMD [ "npm" "start" ]
