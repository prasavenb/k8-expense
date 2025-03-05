FROM node:20.18.3-alpine3.21
EXPOSE 8080
ENV DB_HOST=mysql
RUN addgroup -s expense && adduser -s expense -G expense
RUN mkdir /opt/service
RUN chown -R expense:expense /opt/server
WORKDIR /opt/server
COPY package.json .
COPY *.js .
RUN npm install
USER expense
CMD [ "node", "index.js" ]
