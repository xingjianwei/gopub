FROM alpine
MAINTAINER lsj86@qq.com

# ENV DOWN_URL https://github.com/lisijie/gopub/releases/download/v2.0.1/gopub-v2.0.1-linux-amd64.tar.gz
COPY gopub--linux-amd64.tar.gz /gopub.tar.gz

RUN apk --no-cache add wget \
	&& mkdir gopub && cd gopub \
	&& tar fxz /gopub.tar.gz && rm -f /gopub.tar.gz

CMD ["/gopub/gopub"]