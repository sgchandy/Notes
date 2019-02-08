
##### Delete specific containers
> docker rm <image_name1> <image_name2>

##### Delete all containers
> docker rm $(docker ps -a -q)


##### Delete specific images
> docker rmi <image_name1> <image_name2>

##### Delete all images
> docker rmi $(docker images -q)
