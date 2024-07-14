FROM texlive/texlive:latest-full
# ARG UID=10001

RUN useradd \
    --comment "" \
    --home-dir "/home" \
    --no-create-home \
    --shell "/bin/bash" \
    --uid "${UID}" \
    pdfuser

RUN apt-get update && apt-get install -y \
    git perl git-lfs inkscape openssh-server\
    && rm -rf /var/lib/apt/lists/* \
    && apt-get clean \
    && apt-get autoremove -y \
    && rm -rf /var/lib/apt/lists/* \
    && rm -rf /tmp/*
    
# USER pdfuser

# RUN echo welcome to WebLaTeX2.0