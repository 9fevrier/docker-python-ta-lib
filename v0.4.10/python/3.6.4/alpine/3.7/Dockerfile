# 9fevrier/python-ta-lib:0.4.17_python3.7.0-alpine3.8_20180730
# ============================================================

FROM python:3.6.4-alpine3.7
MAINTAINER contact@9fevrier.com

ENV PYTHON_TA_LIB_VERSION 0.4.10

USER root
WORKDIR /tmp

RUN apk add --no-cache --virtual .build-deps \
        musl-dev \
        linux-headers \
        gcc \
        g++ \
        make \
        curl \
    && cd /tmp \
    && curl -L -O http://prdownloads.sourceforge.net/ta-lib/ta-lib-0.4.0-src.tar.gz \
    && tar -zxf ta-lib-0.4.0-src.tar.gz \
    && cd ta-lib/ \
    && ./configure --prefix=/usr \
    && make \
    && make install \
    && pip3 install setuptools numpy \
    && pip3 install ta-lib==${PYTHON_TA_LIB_VERSION} \
    && apk del .build-deps \
    && rm -rf /root/.cache \
              /tmp/* \
              /var/cache/apk/* \
              /var/lib/apk/lists/*

WORKDIR /root

CMD python3
