FROM node:22

RUN apt update && apt install -y vim moreutils
RUN npm install -g nodemon sequelize sequelize-cli pg pg-hstore eslint ts-node 

WORKDIR /app
COPY . /app
RUN npm install

ENTRYPOINT [ "ts-node", "src/index.ts" ]
