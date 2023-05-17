FROM node:16-alpine

COPY package.json .
RUN rm -rf node_modules/ .next/* && npm install --legacy-peer-deps
COPY . .

RUN npm run build

CMD ["npm", "run", "start"]