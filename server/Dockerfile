# PRODUCTION DOCKER FILE

# Use an existing docker image as a base
FROM node:alpine

WORKDIR '/app'

# copy source files (just package.json) from local folder to container file system
# then install 
COPY ./package.json ./
RUN  npm install

# leave in for production docker file or if we 
# don't use docker-compose
COPY ./ ./


# Tell thee image what to do when it starts 
# as a container
CMD ["npm", "run", "start"]