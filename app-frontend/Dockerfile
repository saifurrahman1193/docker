FROM node:14.5.0-alpine
WORKDIR /app
COPY . .
RUN npm install
RUN npm run build
# ENTRYPOINT npm start
# CMD ["npm", "start"]