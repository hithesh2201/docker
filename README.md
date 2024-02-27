# docker
learning docker basics
https://docs.docker.com/engine/install/centos/
sudo yum install -y yum-utils
sudo yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo
sudo yum install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin -y
sudo systemctl start docker
sudo usermod -aG docker centos
logout and login now u are able to use docker centos user 
for i in mongodb catalogue web user shipping payment mysql cart ; do cd $i ; docker build -t $i:v1 .;cd ..;done
