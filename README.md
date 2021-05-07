## Atlassian products running on one node via docker compose without atlassian-agent

**DO NOT USE DIRECTLY.** These are template file. Do not just clone and run without check.

By default, this repo is placed at `/opt/atlassian` so that the network name is `atlassian_network`. Data will be stored at `postgres` and `application-data` sub directory.

The docker-compose file at root directory is used to start postgres and create network which will be used by any other services.
Every sub directory held one docker-compose file which could be used to start a service. In attention, you need to create database&user yourself.

*Atlassian-agent.jar is a private developing tool which could speed up network connection in particular places. Just delete that.*