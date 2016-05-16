FROM ppc64le/ubuntu 

# gcc for cgo
RUN apt-get update && apt-get install -y --no-install-recommends golang \
	git \
	openssl \
	ca-certificates \
	make \
	gcc  

ENV GOLANG_VERSION 1.6.2

ENV GOPATH /go
ENV PATH $GOPATH/bin:/usr/local/go/bin:$PATH

RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
WORKDIR $GOPATH

