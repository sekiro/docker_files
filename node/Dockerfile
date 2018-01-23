FROM node:8.9.4

RUN export uid=1000 gid=1000 && \
echo "node:x:${uid}:${gid}:node,,,::/bin/bash" >> /etc/passwd && \
echo "node:x:${uid}:" >> /etc/group
USER node
CMD ["/bin/bash"]
