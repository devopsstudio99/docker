# base
FROM node:alpine
# Add maintainer info
MAINTAINER myname@example.com
# Add lab
LABEL OS=alpine
#mount mnt directory
VOLUME /mnt
# /usr/app will create automatic if it not existed
WORKDIR /usr/app
COPY ./package.json  ./
# change owner directory /usr/app to user node
RUN chown -R node:node /usr/app
USER node
# Install node
RUN npm install
# Set environment variable
ENV ENVIRONMENT="development"
COPY ./index.js ./
# cmd
CMD ["npm", "start"]
#export container port
EXPOSE 8080

