# Recipes 
recipes for all kind of crap

# Kubernetes

### fire up a temporary interactive pod with bash

    > kubectl run my-shell --rm -i --tty --image ubuntu -- bash
    
now run the following lines to install the package of your choice, for example **curl**

    >  apt-get update
    >  apt-get install curl
    
now you can communicate with pods from within kubernetes (another alternative to `port-forward`)
or run bash scripts within a pod, etc...


to exit and delete the pod run

    > exit 
