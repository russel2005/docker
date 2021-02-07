To run your image

docker run memcached # run your image
And this:

docker run -d -p 8080:80 myapp 
Runs your image that you tagged "myapp" in the background (-d) and directs traffic from port 8080 to your container's port 80 (-p 8080:80 AKA :)

use docker ps to list running containers

Run and mount the folder on the host named '/home/adam/data' to a folder in the container accessible at '/data/'

docker run -v /home/adam/data:/data debian ls /data
Inspect the volumes for running containers

docker inspect -f {{.Volumes}} container-test
