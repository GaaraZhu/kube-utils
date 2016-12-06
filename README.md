# kube-utils
Some bash scripts to make our life easier to use Kubernetes

## How to use it
1. tail logs of container whose name is like `tester` in dev cluster
```
kdlog tester
```

2. tail logs(from most recent 20 lines) of container whose name is like `tester` in us cluster
```
kpuslog tester 20
```

3. describe a pod in dev cluster whose name is like `tester`
```
kdds pod tester
```

4. describe a configmap in us cluster whose name is like `tester`
```
kpusds configmap tester
```

5. describe a deployment in eu cluster whose name is like `tester`
```
kpeuds deployment tester
```

6. get all images in us cluster
```
kit us
```

## How to install it
* Download the `.ku` file to your local directory(`~/.ku` for example)
* Modify your `~/.bashrc` file to import it.
```
. ~/.ku
```
* Reload your bashrc file
```
source ~/.bashrc
```
