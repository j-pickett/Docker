FROM 	ruby

RUN 	apt-get update && gem install rails && gem install bundler
RUN	apt-get install nodejs -y
RUN	apt-get install sqlite3 -y
RUN	mkdir /opt/app

ONBUILD WORKDIR	/opt/app
ONBUILD ADD	./opt/app
ONBUILD EXPOSE	3000
ONBUILD RUN	gem install
ONBUILD RUN	rake db:migrate
ONBUILD RUN	rake db:seed
