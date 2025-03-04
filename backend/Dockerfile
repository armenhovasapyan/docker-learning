FROM node:18-alpine

WORKDIR /app

COPY package.json .
COPY package-lock.json .

RUN yarn install

COPY . .

EXPOSE 8000

CMD [ "yarn", "start" ]

# docker container inspect mongodb
# docker run --name mongodb -d --rm --network todo-net -v data:/data/db mongo

# docker build -t todoapp .
# docker run --name todo-app --rm -v $(pwd)/src:/app/src --network todo-net -p 8001:8000 todoapp

# docker build -t frontend .
# docker run --name react-todo -it --rm -p 3000:3000 -v $(pwd)/src:/app/src frontend

# docker network ls
# docker network create todo-net
