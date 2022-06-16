# NginxproxyManager-K8S

- Convert docker-compose.yml to yaml on K8S Use Kompose tools:
source: https://kubernetes.io/docs/tasks/configure-pod-container/translate-compose-kubernetes/

- create NFS server to share volume for Pods

some issues: 
- https://github.com/rancher/rancher/issues/25169
- install on all nodes: sudo apt install nfs-common
- set full permision for NFS data share : /nfs/data *(rw,sync,no_subtree_check,no_root_squash)
- https://github.com/kubernetes/kubernetes/issues/54601

....