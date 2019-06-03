# Use an existing docker
FROM alpine

# download
RUN apk add --update redis
RUN apk add --update gcc
# what to do when start

CMD ["redis-server"]
