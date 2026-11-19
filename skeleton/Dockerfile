
FROM node:20-alpine

WORKDIR /app

ENV NODE_ENV=production
ENV HOSTNAME=0.0.0.0

COPY package*.json ./

RUN npm install --include=dev

COPY . .

RUN npm run build

RUN mkdir -p .next/standalone/.next

RUN cp -r .next/static .next/standalone/.next/static

RUN cp -r public .next/standalone/public

EXPOSE 3000

CMD ["node", ".next/standalone/server.js"]


