---
id: create-volume
title: Create Volume
sidebar_label: Create Volume
---

A volume can be created by the following YAML. User should ensure that the corresponding StorageClass already exists.

```yaml
apiVersion: v1
kind: PersistentVolumeClaim
metadata:
  name: iomesh-example-pvc
spec:
    storageClassName: iomesh-example-sc
  accessModes:
    - ReadWriteOnce
  resources:
    requests:
      storage: 10Gi
```
