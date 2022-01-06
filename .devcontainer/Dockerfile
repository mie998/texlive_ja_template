FROM mie999/ubuntu-texlive-ja:latest

RUN apt-get update && apt-get install -y \
    git \
    cpanminus \
    texlive-extra-utils \
    make \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*
    
# INSTALL pandoc
RUN wget https://github.com/jgm/pandoc/releases/download/2.16.2/pandoc-2.16.2-1-amd64.deb \
    && dpkg -i pandoc-2.16.2-1-amd64.deb \
    && rm pandoc-2.16.2-1-amd64.deb

RUN cpanm Log::Log4perl Log::Dispatch::File YAML::Tiny File::HomeDir Unicode::GCString
