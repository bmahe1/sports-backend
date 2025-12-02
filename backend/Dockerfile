FROM node:18

WORKDIR /app

COPY package.json .
COPY products.json .
COPY server.js .

RUN npm install

EXPOSE 3000

CMD ["node", "server.js"]
