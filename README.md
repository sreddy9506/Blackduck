# Hub Docker Orchestration Files/Documentation

This repository will contain orchestration files and documentation for using the individual Hub Docker containers. 

## Important Upgrade Announcement
 
Customers upgrading from a version prior to 4.2, will need to perform a data migration as part of their upgrade process.  A high level description of the upgrade is located in the Important_Upgrade_Announcement.md file in the root directory of this package.  Detailed instructions to perform the migration located in the individual README.md doc file in the directory for the each orchestration method folder.

## Previous Versions

Previous versions of Hub orchestration files can be found on the 'releases' page:

https://github.com/blackducksoftware/hub/releases

## Location of Docker Hub images:

* https://hub.docker.com/r/blackducksoftware/hub-cfssl/ 
* https://hub.docker.com/r/blackducksoftware/hub-webapp/
* https://hub.docker.com/r/blackducksoftware/hub-registration/
* https://hub.docker.com/r/blackducksoftware/hub-solr/
* https://hub.docker.com/r/blackducksoftware/hub-logstash/
* https://hub.docker.com/r/blackducksoftware/hub-postgres/
* https://hub.docker.com/r/blackducksoftware/hub-zookeeper/
* https://hub.docker.com/r/blackducksoftware/hub-jobrunner/
* https://hub.docker.com/r/blackducksoftware/hub-nginx/
* https://hub.docker.com/r/blackducksoftware/hub-documentation/

# Running Hub in Docker

Swarm (mode), Compose, 'docker run', Kubernetes, and OpenShift are supported are supported in Hub 4.2.1. Instructions for running each can be found in the archive bundle:

* docker-run - Instructions and files for running Hub with 'docker run'
* docker-swarm - Instructions and files for running Hub with 'docker swarm mode'
* docker-compose - Instructions and files for running Hub with 'docker-compose'
* kubernetes - Instructions and files for running Hub with Kubernetes
* openshift - Instructions and files for running Hub with OpenShift

## Requirements

### Orchestration Version Requirements

Hub has been tested with:

* Docker 17.03.x
* Docker 17.06.x
* Kubernetes 1.6
* Kubernetes 1.7
* OpenShift Enterprise 3.5

### Hardware Requirements (for Docker Run and Docker Compose)

This is the minimum hardware that is needed to run a single instance of each container. The sections below document the individual requirements for each container if they will be running on different machines or if more than one instance of a container will be run (right now only Job Runners support this).

* 4 CPUs
* 16 GB RAM

### Hardware Requirements (for Docker Compose, Kubernetes, and OpenShift)

This is the minimum hardware that is needed to run a single instance of each container. The sections below document the individual requirements for each container if they will be running on different machines or if more than one instance of a container will be run (right now only Job Runners support this).

* 4 CPUs
* 20 GB RAM

Also note that these requirements are for Hub and do not include other resources that are required to run the cluster overall.

