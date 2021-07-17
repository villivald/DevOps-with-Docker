FROM node:14

EXPOSE 5000

WORKDIR /usr/src/app

RUN curl -sL https://deb.nodesource.com/setup_14.x | bash

RUN apt install -y nodejs

RUN node -v

RUN npm install -g serve

COPY . .

ENV REACT_APP_BACKEND_URL=http://localhost:8080

RUN npm install

RUN npm run build

CMD [ "serve", "-s", "-l", "5000", "build" ]
