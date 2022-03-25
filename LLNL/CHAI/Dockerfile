FROM ghcr.io/rse-ops/cuda-ubuntu-20.04:cuda-11.0.3

# docker build -t chai .

RUN apt-get update && \
    apt-get install -y unzip gfortran && \ 
    spack compiler find && \
    spack install chai
