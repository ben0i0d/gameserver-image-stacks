FROM eoelab.org:1032/build-image-stacks/mcsm-image-stacks/mcsm:base

SHELL ["/bin/bash", "-o", "pipefail", "-c"]

USER root

RUN curl -s https://repos.azul.com/azul-repo.key | gpg --dearmor -o /usr/share/keyrings/azul.gpg && \
    echo "deb [signed-by=/usr/share/keyrings/azul.gpg] https://repos.azul.com/zulu/deb stable main" | tee /etc/apt/sources.list.d/zulu.list && \
    apt-get update --yes && apt-get install --yes --no-install-recommends zulu17-ca-jre-headless && \
    apt-get clean && rm -rf /var/lib/apt/lists/* 
