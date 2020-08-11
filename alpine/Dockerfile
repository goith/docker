FROM alpine:3.11.6

RUN apk upgrade \
    && sed -i 's/dl-cdn.alpinelinux.org/mirrors.aliyun.com/g' /etc/apk/repositories \
    && apk add --no-cache ca-certificates bash git tcpdump rsync tzdata curl \
    && echo 'hosts:          files dns' > /etc/nsswitch.conf

# 时区
ENV TZ Asia/Shanghai
