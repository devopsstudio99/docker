# base
FROM node:alpine

# /usr/app will create automatic if it not existed
WORKDIR /usr/app
# Install node
COPY ./package.json  ./
RUN npm install
ENV ENVIRONMENT="development"
COPY ./index.js ./

# cmd
CMD ["npm", "start"]

