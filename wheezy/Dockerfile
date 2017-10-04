FROM python:2.7.13-wheezy

RUN bash -c "pushd /tmp && \
 curl -O https://cmake.org/files/v2.8/cmake-2.8.10.tar.gz && \
 tar xzf cmake-2.8.10.tar.gz && cd cmake-2.8.10 && \
 ./configure && make && make install && \
 popd && \
 rm -rf /tmp/cmake-2.8.10 /tmp/cmake-2.8.10.tar.gz"

CMD bash
