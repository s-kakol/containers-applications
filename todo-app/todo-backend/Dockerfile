FROM node:16

WORKDIR /usr/src/todo-app

COPY --chown=node:node . .

RUN npm ci --only=production

ENV DEBUG=todo-app:*

USER node

CMD npm start