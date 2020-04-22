MAINTAINER megamanics <github.com/megamanics>
FROM alpine:latest as slim
RUN apk add --update curl && rm -rf /var/cache/apk/*

FROM scratch
COPY --from=slim /bin/curl /bin/curl
ENTRYPOINT ["/bin/curl"]
