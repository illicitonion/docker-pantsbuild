FROM python:2.7.13-wheezy

RUN bash -c "pushd /tmp && \
 curl -O https://cmake.org/files/v3.8/cmake-3.8.0.tar.gz && \
 tar xzf cmake-3.8.0.tar.gz && cd cmake-3.8.0 && \
 ./configure && make && make install && \
 popd && \
 rm -rf /tmp/cmake-3.8.0 /tmp/cmake-3.8.0.tar.gz"

RUN bash -c "tar -C /usr/local -xzf <(curl https://binaries.pantsbuild.org/bin/go/linux/x86_64/1.7.6/go.tar.gz)"

ENV PATH="${PATH}:/usr/local/go/bin"

CMD bash
