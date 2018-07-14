# Initial setup

* Install docker, see https://docs.docker.com for further information
* Make sure it runs, use the docker hello world example for that
* Run `docker-compose build` in this directory to build the required images
* Run `docker-compose up` to start the servers
* Run `./couchdb/setup-initial-database.sh` in order to do set up a minimal database as required for this project

# What it provides
* At http://localhost/ the static html / js / css code is shown
* At http://localhost/experiment-results/ there is the endpoint for storing results
* At http://localhost:5984/_utils/ you can reach the CouchDB GUI

# What is currently not covered
* No security whatsoever. During the startup CouchDB claims that only other containers and the docker host can reach the CouchDB endpoint in case of a normal setup.
* The extraction of the JSON documents from the database are part of the evaluation at a later point
