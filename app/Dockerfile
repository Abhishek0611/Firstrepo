FROM node:8

WORKDIR /usr/src/app

COPY app/package-lock.json ./
COPY app/package.json ./
RUN npm ci --only=production

COPY . .

EXPOSE 8080
CMD [ "npm", "start" ]
