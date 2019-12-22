# kops-nvidia-device-plugin

fork of https://github.com/kubernetes/kops/tree/master/hooks/nvidia-device-plugin/image

# build & push

```
docker build -f Dockerfile -t intelligencebankcom/nvidia-device-plugin:1.0.1 ./
docker push intelligencebankcom/nvidia-device-plugin:1.0.1
```

in kops cluster template

```
spec:
  hooks:
  - execContainer:
      image: intelligencebankcom/nvidia-device-plugin:1.0.0
```
