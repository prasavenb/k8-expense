FROM node:20
RUN mkdir /opt/service
WORKDIR /opt/service
COPY package.json .
COPY *.js .
RUN npm install
CMD [ "node", "index.js" ]
ENV DB_HOST=mysql