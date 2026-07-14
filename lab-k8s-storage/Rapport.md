# ## Lab

## 1. Use `emptyDir` storage

```bash
# 1️⃣ Start a Docker container running Nginx
docker run -d --name nginx‑svc nginx:latest

# 2️⃣ Launch a local Kubernetes cluster with Minikube
minikube start

# 3️⃣ Deploy the manifest that creates the Nginx pod
kubectl apply -f <your‑manifest>.yaml

# 4️⃣ Open an interactive shell inside the newly created pod
kubectl exec -it nginx‑empty‑dir-65ff95686f-5rkqv -- /bin/bash
```

![](local-images/4406a2f004d3842296710b42b1248355b9c5163a.png)

![](local-images/3d872a47583c1900c6aef32874cf6386ebbadce2.png)

![](local-images/b674ef4735359cde09f3c7497ba69c189e52380c.png)

## 2. Use `hostPath` storage

![](local-images/54f94c49cdc819e64e4dc4ecebe648e14e9b6e38.png)

![](local-images/54a36a05d8342dff58433977aaaa3d12993795ee.png)

![](local-images/ffb8c33039257d7504d8e32c61fa587f61c44a37.png)

## 3. Use PersistentVolume

![](local-images/b502f739c8e4e346177be2728a47af3d6ca1620e.png)

## Bonus tasks

Secret volume

![](local-images/ab3fae21ac835e07948c584c1ad77a2e542e9af7.png)

ConfigMap

![](local-images/c4451ff279259a9818a0cf630694182bda930a0e.png)

## Bilan

- A possible application int he real world of storage in kubernetes is deploying an infrastructure with an optimize infrastructure based on persistent and ephemeral storage. Being able to handle storage persistance with ease or almost automatically is a break-through. For example, a queue storage type can be mounted to handle an overload of queries of a SaaS.

- This is Build, deployment and scale phases. Kurbernetes give access to handling these phases with ease.

- This is not a difficulty but some tasks that take a little bit more time than expected. Knowing the syntax can be time-consuming, whilst, without doubt, after knowing it, it will be pleasant.

- Building several types of file. Understanding and coding YAML. Getting experience with IaC. Benefit of ease using kubernetes. K8s is a tremendous system.
