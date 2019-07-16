FROM node:12-slim

WORKDIR /app

COPY . .

RUN npm install 

COPY . .

#EXPOSE 8080 

ENTRYPOINT ["node","Index.js"]
