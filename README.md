FROM node:18-alpin
WORKDIR /app
COPY package*.json ./
RUN npm ci --only=
COPY . .
CMD ["node", "index.js"]
