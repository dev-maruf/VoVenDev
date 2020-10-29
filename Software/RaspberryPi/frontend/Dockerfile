FROM balenalib/raspberrypi3-node
ENV NODE_ENV=production
WORKDIR /app
COPY package*.json ./
COPY .next ./.next
COPY public ./public
RUN install_packages next

EXPOSE 3000
CMD npm run start
