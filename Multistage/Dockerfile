FROM node:10 

WORKDIR /app

COPY ./TeamAPoolProjectUI/* .

RUN npm install

RUN npm install -g @angular/cli=7.3.9

FROM node:12-slim

WORKDIR /app

COPY ./TeamAPoolProjectBackend/* .

RUN npm install

ENTRYPOINT ["ng serve --host 0.0.0.0", "node", "Index.js"]


