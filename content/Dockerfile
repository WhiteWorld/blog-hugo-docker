FROM debian:jessie

RUN apt-get update && apt-get install --no-install-recommends -y ca-certificates git-core
RUN git clone https://github.com/WhiteWorld/blog.whiteworld.me.git /src
VOLUME ["/src"]
COPY ./start.sh /
RUN ["chmod", "755", "/start.sh"]
ENTRYPOINT ["/start.sh"]
