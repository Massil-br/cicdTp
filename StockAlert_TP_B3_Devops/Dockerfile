FROM node:18-alpine

# Mettre à jour les packages Alpine pour corriger les CVE
RUN apk upgrade --no-cache

WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
EXPOSE 3000
CMD ["node", "app.js"]