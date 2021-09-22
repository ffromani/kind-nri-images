# kind-images

### CRIO images

There are images published with CRIO and latest stable Kind versions, the Kubernetes version used is the latest stable published by Kind.

TODO: publish the images and link the instructions
Reference: https://gist.github.com/aojea/bd1fb766302779b77b8f68fa0a81c0f2

### Usage: cri-o

```
# Download kind configuration file to patch the kubelet runtime in order to use CRIO instead of containerd
wget https://raw.githubusercontent.com/fromanirh/kind-nri-images/master/kind-crio.yaml

# Create the cluster with the customized Kind node image
kind create cluster --name crio --image ${IMAGE} --config kind-crio.yaml 
```

### Acknowledgements

This repo is heavily based on the work done on https://github.com/aojea/kind-images


