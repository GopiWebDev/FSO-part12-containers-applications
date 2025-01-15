FROM node

WORKDIR /usr/src/app/backend

COPY --chown=node:node . .

RUN npm ci --omit=dev

ENV DEBUG=backend:*

USER node

CMD ["npm", "start"]