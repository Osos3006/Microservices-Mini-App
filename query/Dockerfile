# specify a base image 
FROM node:14-alpine 

# set the workdir

WORKDIR /app 

# add the needed files package.json , index.js ... etc

COPY ./package.json .

# install some dependencies 
RUN npm install 

COPY ./ ./


# default command 
CMD ["npm" , "start"]