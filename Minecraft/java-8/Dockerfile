FROM eoelab.org:1032/build-image-stacks/gameserver-image-stacks/gameserver:base
RUN wget -qO - https://adoptopenjdk.jfrog.io/adoptopenjdk/api/gpg/key/public | \
    gpg --no-default-keyring --keyring gnupg-ring:/etc/apt/trusted.gpg.d/adoptopenjdk.gpg --import - && \ 
    chown _apt /etc/apt/trusted.gpg.d/adoptopenjdk.gpg
RUN add-apt-repository --yes https://adoptopenjdk.jfrog.io/adoptopenjdk/deb/
RUN apt-get update && apt-get install adoptopenjdk-8-hotspot
