### 1. **Getting the pod's log in K3s**
* Displaying the logs of the pod
* Helps to Identify the errors of the particular pod
---
### 2. **Basic Syntax**
**Command**
* Displaying the log of the pod
```
 kubectl logs <pod-name>
```
---
### 3. **Parameters & Options**
| Parameter | Type    | Description         |
| --------- | ------- | ------------------- |
| `-n`  |  flag  |  Gets the pods created inside the particular namesapce       |
---
### 4. **Common Patterns or Use Cases**
* Getting the logs for the pod deployed inside the namespace
```
kubectl logs site-pods-cdsi783 -n lenscx
```