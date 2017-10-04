FROM python:2.7.13-wheezy

RUN bash -c "pushd /tmp && \
 curl -O https://cmake.org/files/v2.8/cmake-2.8.10.tar.gz && \
 tar xzf cmake-2.8.10.tar.gz && cd cmake-2.8.10 && \
 ./configure && make && make install && \
 popd && \
 rm -rf /tmp/cmake-2.8.10 /tmp/cmake-2.8.10.tar.gz"

RUN bash -c "tar -C /usr/local -xzf <(curl https://binaries.pantsbuild.org/bin/go/linux/x86_64/1.7.6/go.tar.gz)"

ENV PATH="${PATH}:/usr/local/go/bin"

CMD bash
