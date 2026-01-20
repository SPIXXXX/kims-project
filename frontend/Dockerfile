FROM node:20

WORKDIR /app

COPY package*.json ./
RUN npm install

COPY . .

# REQUIRED for Windows + Docker
ENV CHOKIDAR_USEPOLLING=true
ENV CHOKIDAR_INTERVAL=2000

EXPOSE 4200

CMD ["npm", "run", "start"]
