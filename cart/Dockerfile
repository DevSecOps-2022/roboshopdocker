FROM node:20
RUN mkdir -p /app
WORKDIR /app
COPY package.json .
COPY *.js .
RUN npm install
ENV CATALOGUE_HOST=catalogue
ENV REDIS_HOST=redis
ENV CATALOGUE_PORT=8080
CMD ["node", "server.js"]