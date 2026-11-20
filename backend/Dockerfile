FROM node

WORKDIR /app

COPY . .

RUN npm install

CMD ["node", "server.js"]

#docker build ./backend -t backend
#docker run -p 8001:3000 -d backend

#URL a teszthez:http://localhost:8001/api/question