FROM node:8.16.0-alpine
ENV CODE_PUSH_SERVER_VERSION 0.5.4
RUN npm config set registry https://registry.npm.taobao.org/ \
    && npm i -g code-push-server@${CODE_PUSH_SERVER_VERSION} pm2@latest --no-optional

EXPOSE 3000

ENTRYPOINT ["pm2-docker", "start"]
