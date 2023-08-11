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

### portainer 2.18.4

docker swarm 23.0.6

stack: 
https://github.com/valentinedwv/portainer_docker_issues

compose file: compose.yaml 

additional file: compose_override.yaml


### from machines cli

```
earthcube@ip-172-31-2-108:~/portainer_docker_issues$ ./test.sh
[+] Running 2/1
 ✔ Network portainer_docker_issues_default          Created                0.1s 
 ✔ Container portainer_docker_issues-hello_world-1  Created                0.1s 
Attaching to portainer_docker_issues-hello_world-1
portainer_docker_issues-hello_world-1  | extra HELLO WORLD
portainer_docker_issues-hello_world-1 exited with code 0
earthcube@ip-172-31-2-108:~/portainer_docker_issues$ 
```


/var/run/docker.sock

 docker compose version
Docker Compose version v2.17.3

