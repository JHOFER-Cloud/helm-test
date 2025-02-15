Result should be:

![image](https://github.com/user-attachments/assets/54643978-1d1e-4c5d-810c-e6d0e1dfc121)

```bash
kubectl get secret test-apache-secret -n test-apache -o yaml
apiVersion: v1
data:
  TEST_USERNAME: VEVTVF9VU0VSTkFNRV9TRUNSRVQ=
kind: Secret
metadata:
  annotations:
    kubectl.kubernetes.io/last-applied-configuration: |
      {"apiVersion":"v1","data":{"TEST_USERNAME":"VEVTVF9VU0VSTkFNRV9TRUNSRVQ="},"kind":"Secret","metadata":{"annotations":{},"name":"test-apache-secret","namespace":"test-apache"},"type":"Opaque"}
  creationTimestamp: "2025-02-15T15:06:50Z"
  name: test-apache-secret
  namespace: test-apache
  resourceVersion: "5311292"
  uid: 2df3996b-f8a8-4d15-ba0d-5f6fd8c96583
type: Opaque
```
