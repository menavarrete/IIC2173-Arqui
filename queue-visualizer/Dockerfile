FROM node:8-alpine

WORKDIR /queue-visualizer

COPY package.json .
RUN yarn --production=true --frozen-lockfile --non-interactive

COPY . .

ENV PORT 80
EXPOSE 80

CMD ["yarn", "start"]
