FROM balenalib/raspberrypi3-node
ENV NODE_ENV=production
WORKDIR /app
COPY package*.json ./
COPY .next ./.next
COPY public ./public
RUN npm install next

EXPOSE 3000
CMD npm run start
