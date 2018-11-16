FROM alpine:3.8 AS build
RUN apk add --no-cache alpine-sdk
WORKDIR /bin
COPY . /bin
RUN gcc -Wall hellohi.c -o hellohi
FROM alpine:3.8
COPY --from=build /bin/hellohi /bin/hellohi
CMD /bin/hellohi
