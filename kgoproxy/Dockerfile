FROM ghcr.io/goproxy/goproxy:latest

ENV GOPROXY=https://goproxy.cn

VOLUME [ "/data/cacher_dir", "/data/temp_dir"]

RUN export GOPROXY=$GOPROXY

ENTRYPOINT ["/usr/local/bin/goproxy", "-address", ":8080", "-cacher-dir", "/data/cacher_dir", "-temp-dir", "/data/temp_dir"]

EXPOSE 8080