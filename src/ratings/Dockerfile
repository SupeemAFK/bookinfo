FROM node:14-alpine

WORKDIR /app

COPY package*.json .

RUN npm install

COPY . .

EXPOSE 9080

CMD ["node", "ratings.js", "9080"]
