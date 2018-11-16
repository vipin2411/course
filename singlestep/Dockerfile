FROM alpine:3.8
RUN apk add --no-cache alpine-sdk
WORKDIR /bin
COPY . /bin
RUN gcc -Wall hellohi.c -o hellohi
CMD /bin/hellohi
