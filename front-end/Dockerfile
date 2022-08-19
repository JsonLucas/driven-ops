FROM node:16

WORKDIR /app

COPY . .
RUN yarn
RUN yarn build
RUN mkdir -p /var/www/html
RUN mv build/* /var/www/html

WORKDIR /

RUN rm -rf /app

ENV REACT_APP_BASE_URL=http://localhost:5000