FROM node:21.7-alpine

WORKDIR /app.

EXPOSE 3000

COPY package.json package-lock.json /app./

RUN npm install --silent

COPY . /app./

CMD ["npm", "start"]