FROM ghcr.io/rse-ops/cuda-ubuntu-20.04:cuda-11.0.3

# docker build -t sw4 .

RUN apt-get update && \
    apt-get install -y unzip gfortran && \ 
    spack compiler find && \
    spack install sw4lite && \
    apt-get install -y libcurl4-openssl-dev libssl-dev && \
    spack install liblas lapackpp && \
    git clone --depth 1 https://github.com/geodynamics/sw4 /code
WORKDIR /code
RUN . /opt/spack/share/spack/setup-env.sh && \
    spack load && \
    spack load openblas && \
    spack load openmpi && \
    cp configs/make.linux configs/make.inc && \
    make EXTRA_LINK_FLAGS="$(pkg-config --libs openblas) -lgfortran"
