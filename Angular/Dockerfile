FROM node:10 AS build

WORKDIR /build

COPY . .

RUN NG_CLI_ANALYTICS=ci npm install -g @angular/cli

RUN NG_CLI_ANALYTICS=ci npm install

RUN npm run build

RUN ls dist

#-----------------------------------------------------

FROM nginx:alpine

WORKDIR /app

COPY --from=build /build/dist/TeamAPoolProjectUI .

COPY nginx.conf /etc/nginx/nginx.conf
