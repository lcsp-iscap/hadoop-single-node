# Hadoop Single Node Cluster on Docker.

Following this steps you can build and use the image to create a Hadoop Single Node Cluster containers.

## Creating the hadoop image

     $ git clone https://github.com/rancavil/hadoop-single-node-cluster.git
     $ cd hadoop-single-node-cluster
     $ docker build -t hadoop .

## Creating the container

To run and create a container execute the next command:
     
     $ docker run -d --name myhadoop -p 9864:9864 -p 9870:9870 -p 8088:8088 -p 9000:9000 --hostname localhost hadoop

To check if hadoop container is working:

- go to the url in your browser: http://localhost:9870
