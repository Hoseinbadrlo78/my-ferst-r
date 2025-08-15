FROM node:18-
WORKDIR /app
COPY package*.json ./
RUN npm ci --only=
COPY . .
CMD ["node", "index.js"]
