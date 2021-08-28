FROM node:14.15.0-alpine

WORKDIR /code

COPY . /frontend
RUN npm install

RUN ls

CMD ["npm", "run", "serve"]