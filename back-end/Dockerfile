FROM node:16

WORKDIR /usr/src/drivenops-back

COPY package*.json yarn.lock ./

RUN yarn

COPY . .

ENV PORT=5000

EXPOSE 5000

CMD ["yarn", "dev"]