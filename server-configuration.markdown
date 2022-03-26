# Set up and Configuration for Server


# hadoop
before ./start_container.sh
```
sudo docker network create --driver=bridge hadoop
```
but the thing is, 9000 port not exposed outside of docker. You should add -p 9000:9000 after -p 8088:8088 to start-container.sh script, when starting hadoop-master container.
https://github.com/kiwenlau/hadoop-cluster-docker/issues/38



