FROM node:10 

WORKDIR /appFront

COPY ./TeamAPoolProjectUI/* .

RUN npm install

RUN npm install -g @angular/cli=7.3.9

RUN npm build

FROM node:12-slim

WORKDIR /appBack

COPY ./TeamAPoolProjectBackend/* .

RUN npm install

ENTRYPOINT ["node", "Index.js"]


