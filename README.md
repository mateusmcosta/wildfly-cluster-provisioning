# wildfly-cluster-provisioning
Provisioning a Wildfly modcluster cluster.

## Dependencies
* Git Large Files Storage (https://git-lfs.github.com/)
* VirtualBox
* Vagrant
* Ansible

## mod_cluster

You can download mod_cluster's files on: https://modcluster.io/

## Install Cluster

In the project directory:

    $ vagrant up
    $ ansible-playbook provisioning.yml -i hosts

Access the nodes and start the wildfly with:
    $ vagrant ssh wildfly01
    $ cd /opt/wildfly-21.0.2.Final
    $ ./bin/standalone.sh -b 0.0.0.0

    $ vagrant ssh wildfly02
    $ cd /opt/wildfly-21.0.2.Final
    $ ./bin/standalone.sh -b 0.0.0.0

## Test Cluster
ModCluster url:
<br/>
* http://10.220.60.11/mod_cluster_manager
* http://10.220.60.11/mod_cluster_manager 
* http://sample.teste.com.br/sample-1.0.0/hello
