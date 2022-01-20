FROM mjgargani/puppeteer:trybe1.0
WORKDIR /app/tests
COPY package*.json ./
ADD node_modules.tar.gz ./todo-app/tests
RUN npm install
COPY . . 
CMD [ "npm" "test" ]
