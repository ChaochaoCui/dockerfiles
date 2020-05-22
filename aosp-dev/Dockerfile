FROM ubuntu:14.04
RUN apt-get update && apt-get install -y \
            bc \
            vim \
            git-core \
            gnupg \
            flex \
            bison \
            gperf \
            build-essential \
            zip \
            curl \
            zlib1g-dev \
            gcc-multilib \
            g++-multilib \
            libc6-dev-i386 \
            lib32ncurses5-dev \
            x11proto-core-dev \
            libx11-dev \
            lib32z-dev \
            libgl1-mesa-dev \
            libxml2-utils \
            xsltproc \
            unzip \
            software-properties-common && add-apt-repository ppa:openjdk-r/ppa && apt-get update && apt install -y \
            openjdk-8-jdk apt-file openssh-server && rm -rf /var/lib/lists/*
    
COPY docker_entrypoint.sh /root/docker_entrypoint.sh
ENTRYPOINT ["/root/docker_entrypoint.sh"]
