# Study environment setup

## Kubernetes cluster
To prepare for this exam, a kubernetes cluster is needed for practice. This is installed on a MacBook pro with 16G ram. Therefor im somewhat limited in resources. My lab looks like:

MacBookPro (with Fusion)
- kubemaster (1 core, 4G RAM, 50G disk)
- kubenode1 (1 core, 2G RAM, 50G disk)
- kubenode2 (1 core, 2G RAM, 50G disk)
- utils1 (1 core 1G RAM, 100G disk) for external DNS, NFS, image registry

I found the master wants at least 4G RAM to operate, less will slow down its performance. For the nodes its not that important, since it depends on the workload and there will not be that much bulk.

Since the exam is on Kubernetes v1.14, the lab will have v 1.14 installed, with all default bells and whistles.

## Practice installations on GCS
One of the key elements to this exam is how to install and troubleshoot a cluster. For this i will be using Kelsey Hightower's 'Installing the hard way'.
This work is done on Google Cloud.

## Documentation for installation
For installing Kubernetes v1.14 the following documentation is used:
-
