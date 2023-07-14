FROM node:20-slim

RUN apt-get update -y && apt-get upgrade -y && apt-get install -y vim

RUN npm install -g npm \
				express \
				nodemon

COPY ./backend /app/backend

WORKDIR /app/backend

EXPOSE 3000

CMD ["nodemon", "index.js"]
