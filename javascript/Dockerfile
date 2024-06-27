# build
FROM node:18 as build

WORKDIR /app

COPY src/ .

RUN npm install

RUN npm run build

# run
FROM nginx:1.27.0

COPY --from=build /app/out/ /usr/share/nginx/html
