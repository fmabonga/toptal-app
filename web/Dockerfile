FROM node:19-alpine
ARG PORT=8080
ENV API_HOST=
WORKDIR /usr/src/web
COPY package*.json ./
RUN npm install express & npm install
COPY . .
EXPOSE $PORT
CMD ["npm","start"]