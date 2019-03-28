FROM nginx:latest

COPY index.html /usr/share/nginx/html/index.html
COPY DockerFileEx.jpg /usr/share/nginx/html/DockerFileEx.jpg

RUN curl -fsSLO https://get.docker.com/builds/Linux/x86_64/docker-17.04.0-ce.tgz \
  && tar xzvf docker-17.04.0-ce.tgz \
  && mv docker/docker /usr/local/bin \
  && rm -r docker docker-17.04.0-ce.tgz

EXPOSE 80
