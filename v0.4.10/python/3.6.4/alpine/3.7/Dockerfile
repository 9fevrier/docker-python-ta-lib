# 9fevrier/python-ta-lib:python3.6.4-alpine3.7
# ============================================

FROM python:3.6.4-alpine3.7
MAINTAINER contact@9fevrier.com

ENV PYTHON_TA_LIB_VERSION 0.4.10

RUN apk add --no-cache --virtual build-deps \
        musl-dev \
        linux-headers \
        gcc \
        g++ \
        make \ 
        curl \
    && curl -L -O http://prdownloads.sourceforge.net/ta-lib/ta-lib-0.4.0-src.tar.gz \
    && tar -zxf ta-lib-0.4.0-src.tar.gz \
    && cd ta-lib/ \
    && ./configure --prefix=/usr \
    && make \
    && make install \
    && pip3 install setuptools numpy \
    && pip3 install ta-lib==${PYTHON_TA_LIB_VERSION} \
    && rm -rf ta-lib* \
    && rm -r /root/.cache

CMD python3


