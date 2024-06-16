FROM ghcr.io/tatsumi0000/iosdc2024-pamphlet/texlive-ja:latest

RUN apt update && apt upgrade -y && apt install -y \
    git \
    cpanminus \
    texlive-extra-utils \
    make \
    && apt clean \
    && rm -rf /var/lib/apt/lists/*

RUN cpanm Log::Log4perl Log::Dispatch::File YAML::Tiny File::HomeDir Unicode::GCString