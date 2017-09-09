To delete all containers

            docker rm $(docker ps -a -q)

to delete all images

            docker rmi $(docker images -q)
