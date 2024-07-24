# apps/app1/Dockerfile
FROM node:20-alpine

WORKDIR /usr/src/app

COPY package.json package-lock.json ./
COPY . .

RUN npm i

RUN npm run build:app2

EXPOSE 3000

CMD ["npm", "run", "start:app2"]
