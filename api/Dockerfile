FROM node:19-alpine
ARG PORT=3000
ENV DB= DBUSER= DBPASS= DBHOST= DBPORT=
WORKDIR /usr/src/api
COPY package*.json ./
RUN npm install express 
RUN npm install & apk add postgresql
COPY . .
EXPOSE $PORT
CMD ["npm","start"]