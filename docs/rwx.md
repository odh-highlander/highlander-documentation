# ROX/RWX volume for the shared library

As explained in the [Introduction](solution.md), you need a ROX volume to store the shared library.

Obviously you will need to be able to write into it at some point to populate the library, so in fact what you need is an RWX volume (read write many). It will simply be mounted in a Read-Only mode in the pods that will use the library, and Read-Write in the pod you will use to add modules to the library.

Here are different options.

## CephFS

The reference architecture for this project leverages CephFS through Rook or OpenShift Data Foundation. This directly provides an RWX storageClass that you can use for the library.

## NFS Provisioner

In case you don't have access to CephFS, this project provides a method to install a simple NFS Provisioner and Server. It will create a new StorageClass with RWX capabilities that you will be able to use to create a volume for the library.

You will find all the instructions and code in this repository: [https://github.com/odh-highlander/nfs-server-and-provisioner](https://github.com/odh-highlander/nfs-server-and-provisioner)
