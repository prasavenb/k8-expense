FROM node:20.18.3-alpine3.21
RUN mkdir /opt/service
WORKDIR /opt/service
COPY package.json .
COPY *.js .
RUN npm install
CMD [ "node", "index.js" ]
ENV DB_HOST=mysql