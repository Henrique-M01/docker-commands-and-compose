FROM mjgargani/puppeteer:trybe1.0 AS build

WORKDIR /app/tests

COPY package*.json ./

ADD node_modules.tar.gz ./todo-app/tests

COPY . . 

CMD [ "npm", "test" ]
