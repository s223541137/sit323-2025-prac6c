# SIT323/SIT737 – Task 6.2P: Kubernetes Cluster Interaction

## Overview
This task involved interacting with the Kubernetes cluster hosting the Node.js application using both the `kubectl` CLI and browser.

---

## Steps Followed

### 1. Verified Application Status
- Ran `kubectl get pods` to check pod status
- Ran `kubectl get services` to check service exposure

### 2. Port-Forwarded Local Traffic
- Used `kubectl port-forward` to forward local port 8080 to pod port 3000
```bash
kubectl port-forward pod/nodejs-app-deployment-79746d79fd-p5725 8080:3000
