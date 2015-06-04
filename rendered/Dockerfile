FROM crosbymichael/golang

RUN apt-get update && apt-get install --no-install-recommends -y bzr

RUN go get github.com/spf13/hugo

VOLUME ["/var/www/blog"]

ENTRYPOINT ["hugo"]
CMD ["-w", "-s", "/src", "-d", "/var/www/blog"]
