mvn spring-boot:run -Dserver.port=8083 -Deureka.instance.metadataMap.instanceId=instance3

To generate swagger doc PDF install jRuby
	https://github.com/jruby/jruby/wiki/GettingStarted
	
	
Install Docker from the below link
     https://github.com/docker/toolbox/releases/tag/v1.12.2
    
    Install below docker products: Below products will be in a single executable file, make sure that all are selected or checked while installing.
	    
	    1. docker-machine
	    2. docker-compose
		 3. docker
		 4. docker -v
		 
		 After installing the docker successfully.(All commands are for windows machine)
		 
		 	a. Open docker terminal. It will start the docker-machine automatically.
		   b. Open the git bash or any terminal.
		   c. use following commands before building.
		 
				 i. export DOCKER_HOST=unix:///var/run/docker.sock
				 ii. docker-machine env
				 
				      --------------below will the out put--------------------
				      
				      export DOCKER_TLS_VERIFY="1"
						export DOCKER_HOST="tcp://192.168.99.100:2376"
						export DOCKER_CERT_PATH="C:\Users\abhishek.sharma\.docker\machine\machines\default"
						export DOCKER_MACHINE_NAME="default"
						# Run this command to configure your shell:
						# eval $("C:\Program Files\Docker Toolbox\docker-machine.exe" env)
						
						---------------copy last line and paste to get step ->(iii)---------
				 
				 iii. eval $("C:\Program Files\Docker Toolbox\docker-machine.exe" env)
				 iv. docker-machine restart
				 v. docker images
