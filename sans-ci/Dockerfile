FROM libreflip/deployment:base-armhf
MAINTAINER Katharina Fey <kookie@spacekookie.de>

RUN apt-get install -y wget libpcre3-dev:armhf libudev-dev:armhf
RUN wget http://www.imagemagick.org/download/ImageMagick-7.0.7-30.tar.gz -O ImageMagick.tar.gz && \
        tar xf ImageMagick.tar.gz && \
        cd ImageMagick* && \
        ./configure --prefix=/usr && \
        make -j 4 && \
        make install