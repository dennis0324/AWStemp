FROM node:21 AS production

WORKDIR /usr/src/app
# RUN curl -fsSL https://bun.sh/install | bash

copy package*.json ./
RUN npm install --production=true
COPY . . 
run npm run build

CMD ["npm","run","start:prod"]