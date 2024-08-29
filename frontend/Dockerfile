FROM node:22-bookworm

WORKDIR /home/docker/app

RUN rm -rf .angular/cache

# npm install inside the docker
ADD package.json /tmp/package.json
RUN cd /tmp && npm install
RUN mkdir -p /opt/app && cp -a /tmp/node_modules /opt/app/

CMD ["npm", "start"]

EXPOSE 4200