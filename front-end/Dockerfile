FROM node:16

WORKDIR /usr/src/drivenops-front

COPY package*.json yarn.lock ./

RUN yarn

COPY . .

CMD ["yarn", "start"]