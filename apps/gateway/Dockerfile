FROM node:16-alpine
WORKDIR /app
COPY package*.json tsconfig.json ./
RUN npm ci
COPY src ./src
RUN npm run build
EXPOSE 3000
CMD ["node", "dist/main.js"]
