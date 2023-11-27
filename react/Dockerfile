FROM node:21 AS production

WORKDIR /usr/src/app

copy package*.json ./
RUN npm install --production=true
COPY . . 
run npm run build

CMD ["npm","run","start:prod"]