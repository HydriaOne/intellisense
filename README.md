# Intellisense DevOps Test
## Description
This is a simple command line tool that provides a table output which includes the following details:
* Name of deployments
* Images of each deployment
* Date deployment was updated

We can run this application on docker or in our local pc.

## How to use it

### PreRequisits:

 * Python 3.9 and all the dependences
```
pip install -r requeriments.txt
```
 * Kubectl set up, or a valid kubeconfig file, by default i will use the ~/.kube/config

### Commands:

All namespaces:
```
python3 main.py
```

Specific namespace:
```
python3 main.py -n subsonic
```

Specific namespace & custom configfile:
```
python3 main.py -n subsonic -c kubeconfig
```