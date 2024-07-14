FROM texlive/texlive:latest-full
RUN apt-get update && apt-get install -y \
    git git-lfs perl inkscape openssh-server\
    && rm -rf /var/lib/apt/lists/* \
    && apt-get clean \
    && apt-get autoremove -y \
    && rm -rf /var/lib/apt/lists/* \
    && rm -rf /tmp/*