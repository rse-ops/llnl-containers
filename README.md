# LLNL Containers

Welcome to the LLNL Containers Development Space! This is an [rse-ops Special Project](https://rse-ops.github.io/proposals/proposals/drafts/automated-container-builds/)
that aims to support lab software by creating automated container builds for it.
We will be using the [rse-ops docker-images](https://github.com/rse-ops/docker-images) as bases,
and as we develop container builds, will be synthesizing into GitHub actions that can be more
easily used.

## Organization

Each directory here reflects the Github namespace. If a directory is not present, it already has containers!

- [geodynamics/sw4](geodynamics/sw4)
- [GEOSX/GEOSX](GEOSX/GEOSX): already has [automated builds](https://github.com/GEOSX/thirdPartyLibs/tree/master/docker) on Docker hub under [geosx](https://hub.docker.com/u/geosx).

License
-------

Copyright (c) 2022, Lawrence Livermore National Security, LLC. 
Produced at the Lawrence Livermore National Laboratory.

RADIUSS is licensed under the MIT license [LICENSE](./LICENSE).

Copyrights and patents in the RADIUSS Docker project are retained by
contributors. No copyright assignment is required to contribute to RADIUSS
Docker.

This work was produced under the auspices of the U.S. Department of
Energy by Lawrence Livermore National Laboratory under Contract
DE-AC52-07NA27344.
