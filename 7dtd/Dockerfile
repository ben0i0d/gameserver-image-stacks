FROM eoelab.org:1032/build-image-stacks/gameserver-image-stacks/gameserver:steam
#Ports
EXPOSE 26900 26900/UDP 26901/UDP 26902/UDP 8082 8081 8080

RUN steamcmd +force_install_dir /workspace +login anonymous +app_update 294420 validate +quit
