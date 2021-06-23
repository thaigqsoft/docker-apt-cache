# docker-apt-cache
# Ex
 docker run -d -p 3142 -v ./apt-cacher-ng:/var/cache/apt-cacher-ng --name apt-cache  thaigqsoft/docker-apt-cache
 #
 In Dockerfile
 RUN echo 'Acquire::http { Proxy "http://dockerhost:3142"; };' >> /etc/apt/apt.conf.d/01proxy
