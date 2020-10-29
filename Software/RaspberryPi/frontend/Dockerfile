FROM balenalib/raspberrypi3-node
ENV NODE_ENV=production
WORKDIR /app
COPY --from=build /build/package*.json ./
COPY --from=build /build/.next ./.next
COPY --from=build /build/public ./public
RUN install_packages next

EXPOSE 3000
CMD npm run start
