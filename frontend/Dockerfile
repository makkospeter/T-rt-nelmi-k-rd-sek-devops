FROM node AS build

WORKDIR /app

COPY . .

RUN npm i

RUN npm run build

FROM nginx AS final
COPY --from=build /app/dist /usr/share/nginx/html

#docker build ./frontend -t frontend
#docker run -p 8002:80 -d frontend