FROM node:12-slim

WORKDIR /app

COPY ./TeamAPoolProjectBackend/* .

RUN npm install 

COPY ./TeamAPoolProjectBackend/* .

#EXPOSE 8080 

ENTRYPOINT ["node","Index.js"]
