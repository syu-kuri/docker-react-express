FROM node:20-slim

RUN apt-get update -y && apt-get upgrade -y && apt-get install -y vim

RUN npm install -g npm \
    @testing-library/jest-dom \
    @testing-library/react \
    @testing-library/user-event \
    react \
    react-dom \
    react-scripts \
    web-vitals

COPY ./frontend /app/frontend

WORKDIR /app/frontend

EXPOSE 3000

CMD ["npm", "start"]
