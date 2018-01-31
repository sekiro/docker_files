FROM node:8.9.4

RUN export uid=1000 gid=1000 && \
echo "node:x:${uid}:${gid}:node,,,::/bin/bash" >> /etc/passwd && \
echo "node:x:${uid}:" >> /etc/group
RUN mkdir /app && \
chown node:node /app
USER node
RUN git clone -b develop https://github.com/sekiro/nodejs_back_develop.git /app/ && \
mkdir /app/node_modules && \
cd /app && \
npm install
