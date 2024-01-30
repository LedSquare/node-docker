FROM node:18-bookworm AS builder
# Create app directory
WORKDIR /app

COPY frontend/package*.json /app
# If you are building your code for production
#RUN npm ci --omit=dev && npm run build
RUN npm install

COPY frontend/ /app

EXPOSE 3000

CMD [ "npm", "run", "dev" ]
