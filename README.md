# show issue with additional files

## run in local dev workstation docker

Docker Compose version v2.15.1

```
valentin@MacBook-Pro portainer_docker_issues % ./test.sh
[+] Running 1/1
 ⠿ Container portainer_docker_issues-hello_world-1  Recreated                                                                                                     0.9s
Attaching to portainer_docker_issues-hello_world-1
portainer_docker_issues-hello_world-1  | extra HELLO WORLD
portainer_docker_issues-hello_world-1 exited with code 0
valentin@MacBook-Pro portainer_docker_issues %
 ```

## run in portainer using a docker stack
`HELLO WORLD echo extra HELLO WORLD`

portainer 2.18.4

docker swarm 23.0.6

stack: 
https://github.com/valentinedwv/portainer_docker_issues

compose file: compose.yaml 

additional file: compose_override.yaml





/var/run/docker.sock

 docker compose version
Docker Compose version v2.17.3

