# docker
Docker related files

The project contains several docker modules corrosponding to differnt SCSB projects. In order to build a particular image run the build command as follows from within the module that has the Dockerfile

Ex - Build scsb-solr-client images
docker build -t scsb-solr-client .

In order to build tagged releases of a particular project, run the commanad as follows:

Ex - Build scsb-solr-client v0.6.0 version
sudo docker build --no-cache=true --build-arg TAG='0.6.0' -t scsb-solr-client .

[![HTC](https://github.com/premkumarbalu/docker/blob/logo/htc-global-services-squarelogo.png)]()

