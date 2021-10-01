# 14848_HW2
## Please see screenshots and details in the Docker folder
## First Container
### URLs:

docker pull elizxiong/hellopython:latest

https://hub.docker.com/repository/docker/elizxiong/hellopython


### Dockerfile Contents:

From python:latest

Copy . /usr/src/hw1

WORKDIR /usr/src/hw1

CMD ["python","hello.py"]


<img width="1204" alt="first Docker image" src="https://user-images.githubusercontent.com/60122319/135212981-17798acc-d88f-42ad-b604-8678e00d5f18.png">

### First Container on GCP:

Image URL: 
gcr.io/static-protocol-327314/elizxiong/hellopython@sha256:167a9fbce7df65d29047cfbb6436fc2a3dcfc2c28581a33ca40e49cce85f2618

Cluster Info:

https://console.cloud.google.com/logs/query;query=resource.type%3D%22cloud_run_revision%22%0Aresource.labels.service_name%3D%22hellopython%22%0Aresource.labels.revision_name%3D%22hellopython-00002-lep%22;cursorTimestamp=2021-09-29T02:59:35.799301363Z?project=static-protocol-327314 

### Commands used to deploy container to GCP:
<img width="1188" alt="first_container_to_GCP_commands" src="https://user-images.githubusercontent.com/60122319/135213025-9f2f25f2-947f-4a23-b33d-0aa7af60cbc9.png">

### Run the container on GCP output:
<img width="1272" alt="first_container_GCP_output" src="https://user-images.githubusercontent.com/60122319/135212926-2d8dec44-55c2-4e3c-af0e-832db654f343.png">

## Second Container
### Run the container output:
<img width="872" alt="second container output" src="https://user-images.githubusercontent.com/60122319/135213299-fa2f7b37-9c9e-4ee0-a9cb-33f9b2a4e7c5.png">

### Commands used to get the above result:
<img width="591" alt="second container commands" src="https://user-images.githubusercontent.com/60122319/135554207-1df57932-55b6-4e39-8a8c-38dedac76091.png">

## Extra Credit
### Kubernetes cluster on GCP Output:
<img width="1251" alt="extra_point_output" src="https://user-images.githubusercontent.com/60122319/135213426-948f1f29-06d0-48ab-8ccd-597603df4c64.png">
### Kubernetes Cluster Info:
<img width="1081" alt="GCP_kubernetes_info" src="https://user-images.githubusercontent.com/60122319/135213495-af50aff5-37fc-484e-9877-e406c40d53b7.png">
### Expose the cluser:
<img width="1249" alt="expose_cluster" src="https://user-images.githubusercontent.com/60122319/135213558-b201cc5c-9c79-4a08-acf2-e99d520f9ba5.png">



