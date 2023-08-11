# show issue with additional files

run in local dev workstation docker

```
valentin@MacBook-Pro portainer_docker_issues % ./test.sh
[+] Running 1/1
 ⠿ Container portainer_docker_issues-hello_world-1  Recreated                                                                                                     0.9s
Attaching to portainer_docker_issues-hello_world-1
portainer_docker_issues-hello_world-1  | extra HELLO WORLD
portainer_docker_issues-hello_world-1 exited with code 0
valentin@MacBook-Pro portainer_docker_issues %
 ```

run in portainer using a docker stack

https://github.com/valentinedwv/portainer_docker_issues.


compose.yaml 

additional file:

compose_override.yaml

`HELLO WORLD echo extra HELLO WORLD`
