FROM node:alpine as build
WORKDIR /app
COPY package.json ./
RUN yarn

FROM node:alpine
#RUN apk add nodejs --no-cache
WORKDIR /app
COPY --from=build /app/node_modules ./node_modules
COPY . .
CMD ["npx", "nodemon", "app.js"]