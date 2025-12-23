# specify a base image 
FROM node:14-alpine 

# Add the following lines to fix a bug that prevents create-react-app from working in a docker container 
ENV CI=true
ENV WDS_SOCKET_PORT=0

# set the workdir

WORKDIR /app 

# add the needed files package.json , index.js ... etc

COPY ./package.json .

# install some dependencies 
RUN npm install 

COPY ./ ./


# default command 
CMD ["npm" , "start"]