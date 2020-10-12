For development environments use this provided docker-compose.yml file to run the code in a docker container. The files in your source directory on your host system will be bind mounted into the container's /usr/lib64/python2.7/site-packages/TCGStorageAPI directory

THIS IS TO BE RUN AT THE TOP LEVEL SOURCE PROJECT DIRECTORY FOR IT TO WORK Files that you edit in your source project directory will be used by the container that you started.

To Start the container run the following in the top level directory: sudo docker-compose -f docker/docker-compose.yml up -d

Run the following command to ssh into the docker container to run the code: The name of the container can be found using "sudo docker ps" sudo docker exec -it <name of container> /bin/bash

To stop the container run the following in the top level directory: sudo docker-compose -f docker/docker-compose.yml stop
