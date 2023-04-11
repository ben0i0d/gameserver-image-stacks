FROM eoelab.org:1032/build-image-stacks/gameserver-image-stacks/gameserver:steam
#Ports
EXPOSE 26900 26900/UDP 26901/UDP 26902/UDP 8082 8081 8080

RUN steamcmd && \
    sh -c ‘/bin/echo -e “force_install_dir /workspace” && \
    sh -c ‘/bin/echo -e “login anonymous”  && \
    sh -c ‘/bin/echo -e “app_update 294420”  && \
    sh -c ‘/bin/echo -e “quit”

