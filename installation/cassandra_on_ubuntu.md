
# Installing Cassandra On Ubuntu



## Preparation

Install Development Tools

```bash
  sudo apt-get update
  sudo apt install wget
  sudo apt install make
  sudo apt install gcc
  sudo apt install tcl
  sudo apt install build-essential
```
    
## Install JAVA-11
```bash
  sudo apt-get install openjdk-11-jdk
```
In Case you have different version of JAVA, you should still go ahead and run the above command to install JAVA-11

You will then have multiple version of JAVA installed and you have to select JAVA-11 by running:
```bash
  sudo update-alternatives --config java
```
Then give the integer choice of number that you want
## Create Workstation and Install Cassandra

Create a directory where we will install Cassandra and download Cassandra Binaries

```bash
  cd /
  mkdir apache_cassandra
  cd apache_cassandra
  wget https://dlcdn.apache.org/cassandra/4.1.4/apache-cassandra-4.1.4-bin.tar.gz
  tar -xvf apache-cassandra-4.1.4-bin.tar.gz
  cd apache-cassandra-4.1.4/
```

Start Cassandra
```bash
  bin/cassandra -f -R
  ```
