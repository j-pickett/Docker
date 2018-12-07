FROM	debian

RUN	apt-get update && apt-get upgrade -y && apt-get install bzip2 wget -y && \
	wget http://dl.4players.de/ts/releases/3.0.13.4/teamspeak3-server_linux_amd64-3.0.13.4.tar.bz2 && \
	tar -xvf teamspeak3-server_linux_amd64-3.0.13.4.tar.bz2

WORKDIR	teamspeak3-server_linux_amd64

CMD	["sh", "ts3server_minimal_runscript.sh"]
