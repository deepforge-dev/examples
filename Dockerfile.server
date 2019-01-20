# Dockerfile for running the server itself
FROM deepforge/server
MAINTAINER Brian Broll <brian.broll@gmail.com>

RUN deepforge extensions add deepforge-dev/deepforge-keras

CMD ["deepforge", "start", "--server"]
