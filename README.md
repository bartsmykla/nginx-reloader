Simple tool to send HUP signal to the nginx process when k8s' configmap change.

It's working only on Kubernetes >= 1.13 because it needs this feature:
https://kubernetes.io/docs/tasks/configure-pod-container/share-process-namespace/

If you'll configure **share process namespace** you can add it as a sidecar container, and it should just work