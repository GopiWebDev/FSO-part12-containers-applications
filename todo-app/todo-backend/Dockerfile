FROM node

WORKDIR /usr/src/app/

COPY --chown=node:node . .

RUN npm ci --omit=dev

ENV DEBUG=app:*

USER node

CMD ["npm", "start"]