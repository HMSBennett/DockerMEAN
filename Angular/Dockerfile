FROM node:10

WORKDIR /app

COPY . .

ENV ANGULAR_CLI_VERSION=7.3.9

RUN npm install

RUN npm install -g @angular/cli@${ANGULAR_CLI_VERSION}

#EXPOSE 4200

CMD ng serve --host 0.0.0.0
