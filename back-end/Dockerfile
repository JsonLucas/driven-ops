FROM node:16

WORKDIR /usr/src/drivenops-back

COPY package*.json yarn.lock ./

RUN yarn

COPY . .

ENV PORT=5000 
ENV DATABASE_URL=postgresql://projects:admin@localhost:5432/students

EXPOSE 5000

CMD ["yarn", "dev"]