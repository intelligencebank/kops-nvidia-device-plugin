# kops-nvidia-device-plugin

fork of https://github.com/kubernetes/kops/tree/master/hooks/nvidia-device-plugin/image

# build & push

```
docker build -f Dockerfile -t jiangjingwei/nvidia-device-plugin:1.0.1 ./
docker push jiangjingwei/nvidia-device-plugin:1.0.1
```

in kops cluster template

```
spec:
  hooks:
  - execContainer:
      image: jiangjingwei/nvidia-device-plugin:1.0.0
```
