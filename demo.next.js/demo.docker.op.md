
sudo docker image ls
sudo docker run node_demo

sudo docker ps


# create docker
export con_name=node_demo
export new_con_name=next_demo
sudo docker run -d --name $con_name $con_name  
# clear docker
sudo docker stop $con_name  
sudo docker rm $con_name  
# go into container
sudo docker exec -it $con_name bash
# save container at other name
sudo docker commit $con_name
export Image_Id=f2d2271c133c
sudo docker tag $Image_Id $new_con_name

# build
export con_name=next_d1

sudo docker build -t 'next_d1' .
sudo docker run -d --name $con_name $con_name
sudo docker exec -it $con_name bash
sudo docker image ls
sudo docker ps
sudo docker stop $con_name;sudo docker rm $con_name

# //RUN npx create-next-app@latest create_test -y


