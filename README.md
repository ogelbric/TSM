# TSM
Tanzu Service Mesh

**Creating a Tanzu Service Mesh like this:**

![GitHub](GlobalNameSpace.png)

*Step 1
*Creating 2 Kubernetes clusters in a "system" that has outbound internet access (to get to TSM (Cloud))
*In this case a vCenter 7 install with Kubernetes is used.

*The Kubernetes cluster creation is done as follows 
  *Log onto Supervisor Cluster
    /usr/local/bin/kubectl-vsphere login --vsphere-username administrator@vsphere.local --server=https://192.168.2.1 --insecure-skip-tls-verify
  *Swap Context
    *kubectl config use-context namespace1000
  *Local file for cluster creation
    *kubectl apply -f ./guestcluster1001GA-9workers.yaml.1168tkg21
  *Remote file for cluster creation
    *kubectl apply -f https://github.com/ogelbric/YAML/raw/master/guestcluster1001GA-9workers.yaml.1168tkg21
    
**Create 2 Clusters in TSM**
![GitHub](2clusters.png)
test r


