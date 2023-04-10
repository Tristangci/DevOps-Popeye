FROM node:12-alpine

WORKDIR /app

COPY package*.json ./

RUN npm install --only=production && \
    npm cache clean --force

COPY . .

EXPOSE 80

CMD ["npm", "start"]
