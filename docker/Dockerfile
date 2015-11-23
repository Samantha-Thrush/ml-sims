FROM ipython/scipyserver
MAINTAINER Edward Kim <edward.junhyung.kim@gmail.com>
RUN apt-get update && \
    apt-get -y -q install libfftw3-dev libatlas-base-dev wget vim
RUN pip install --upgrade --no-deps git+git://github.com/Theano/Theano.git && \
    pip install --upgrade --no-deps git+git://github.com/Lasagne/Lasagne.git && \
    pip install --upgrade --no-deps git+git://github.com/dnouri/nolearn.git
RUN pip install --upgrade six pyyaml && \
    cd / && \
    git clone https://github.com/lisa-lab/pylearn2 && \
    cd pylearn2 && \
    python3 setup.py develop

ENV PYLEARN2_DATA_PATH "eog --new-instance"
