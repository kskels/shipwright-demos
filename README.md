#  Shipwright Demos

```bash
oc new-project shipwright-builds
```

# Buildah

```bash
oc apply -f buildah/

oc new-app --name sample-go --image-stream sample-go
oc expose service/sample-go
```

# Buildpacks v3

```bash
oc apply -f buildpacks/

oc new-app --name sample-go --image-stream sample-go
oc expose deploy/sample-go --port 8080
oc expose service/sample-go
```
