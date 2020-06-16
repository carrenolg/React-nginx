################################## Stage 1 - builder
FROM node:alpine as build

# set working directory
WORKDIR /app

# copy everything to /app directory.
COPY ./app /app

# add the node_modules folder to $PATH
ENV PATH /app/node_modules/.bin:$PATH

# install and cache dependencies
RUN yarn

#build the project for production
# set up production environment
RUN yarn build
