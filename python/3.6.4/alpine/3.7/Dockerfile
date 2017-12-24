# 9fevrier/python-ta-lib:python3.6.4-alpine3.7
# ============================================

FROM python:3.6.4-alpine3.7

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
    && pip3 install ta-lib \
    && rm -rf ta-lib* \
    && rm -r /root/.cache

CMD python3


