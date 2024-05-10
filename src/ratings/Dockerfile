FROM node:14-alpine

WORKDIR /usr/src/app

COPY package.json package-lock.json* ./

RUN npm install

COPY . .

EXPOSE 9080

CMD ["node", "ratings.js", "9080"]
