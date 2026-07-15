FROM node:20
RUN mkdir -p /app
WORKDIR /app
COPY package.json .
COPY *.js .
RUN npm install
ENV MONGO_URL="mongodb://mongodb:27017/users"
ENV EDIS_URL='redis://redis:6379'
ENV MONGO=true
CMD ["node", "server.js"]