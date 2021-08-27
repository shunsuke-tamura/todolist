FROM node:14.15.0-alpine

WORKDIR /app

COPY . /app
RUN npm install

RUN ls

CMD ["npm", "run", "serve"]