From:nfcore/base
Bootstrap:docker

%labels
    MAINTAINER Carlos Guzman
    DESCRIPTION Singularity image containing all reqs for the nf-core/chip heinzlab pipeline
    VERSION 1.0dev

%environment
    PATH=/opt/conda/envs/nf-core-chip-1.0dev/bin:$PATH
    export PATH

%files
    environment.yml /

%post
    /opt/conda/bin/conda env create -f /environment.yml
    /opt/conda/bin/conda clean -a
