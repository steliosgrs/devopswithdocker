# Start from the alpine image
FROM node:14-alpine

WORKDIR /path/javascript/app/

COPY ./example-frontend .

RUN npm install

RUN npm run build

RUN npm install -g serve

ENV REACT_APP_BACKEND_URL=http://localhost:9000

EXPOSE 5000

ENTRYPOINT [ "serve", "-s", "-l", "5000", "build" ] 