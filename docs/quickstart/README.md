![PipelineAI Logo](http://pipeline.ai/assets/img/logo/pipelineai-split-black-258x62.png)

### Requirements
* 8GB
* 4 Cores
* Install [Docker](https://www.docker.com/community-edition#/download)
* Python 2 or 3 ([Conda](https://conda.io/docs/install/quick.html) is Preferred)
* (Windows Only) Install [PowerShell](https://github.com/PowerShell/PowerShell/tree/master/docs/installation) 

### Install PipelineAI CLI
```
pip install cli-pipeline==1.5.112 --ignore-installed --no-cache -U
```
Notes: 
* If you have any issues, you may want to create a separate virtualenv or conda environment to isolate the environments.
* You may need to run `pip uninstall -y python-dateutil` if you see an issue related to `pip._vendor.pkg_resources.ContextualVersionConflict`
* This command line interface requires **Python 2 or 3** and **Docker** as detailed above in the Pre-Requisites section.
* You may need to specify `--user` if you have issues.
* If you're having trouble, use one of our support channels [**HERE**](#24x7-support) to let us know!

### PipelineAI Quick Start (CPU and GPU)
Train and Deploy your ML and AI Models in the Following Environments:
* [Docker](/docs/quickstart/docker)
* [Kubernetes](/docs/quickstart/kubernetes)
* [AWS SageMaker](/docs/quickstart/sagemaker)

### Verify Successful PipelineAI CLI Installation
```
pipeline version

### EXPECTED OUTPUT ###
cli_version: 1.5.x    <-- MAKE SURE THIS MATCHES THE VERSION YOU INSTALLED ABOVE

default train base image: docker.io/pipelineai/train-cpu:1.5.0     
default predict base image: docker.io/pipelineai/predict-cpu:1.5.0 
```

### PipelineAI CLI Overview
```
pipeline help

### EXPECTED OUTPUT ###
...
env-conda-activate          <-- Switch to a New Model (Updates Conda Environment)

help                        <-- This List of CLI Commands

predict-http-test           <-- Test Model Cluster (Http-based)

predict-kube-autoscale      <-- Configure AutoScaling for Model Cluster
predict-kube-connect        <-- Create Secure Tunnel to Model Cluster 
predict-kube-describe       <-- Describe Model Cluster (Raw)
predict-kube-endpoint       <-- Retrieve Model Cluster Endpoint 
predict-kube-endpoints      <-- Retrieve All Model Cluster Endpoints
predict-kube-logs           <-- View Model Cluster Logs 
predict-kube-route          <-- Route Live Traffic  
predict-kube-routes         <-- Describe Routes
predict-kube-scale          <-- Scale Model Cluster
predict-kube-shell          <-- Shell into Model Cluster
predict-kube-start          <-- Start Model Cluster from Docker Registry
predict-kube-stop           <-- Stop Model Cluster
predict-kube-test           <-- Test Model Cluster

predict-sage-describe       <-- Describe Model Cluster (SageMaker)
predict-sage-route          <-- Route Live Traffic (SageMaker)
predict-sage-start          <-- Start Model Cluster (SageMaker)
predict-sage-stop           <-- Stop Model Cluster (SageMaker)
predict-sage-test           <-- Test Model Cluster (SageMaker)

predict-server-build        <-- Build Model Server
predict-server-init         <-- Initialize Directory for Model Server Dev
predict-server-logs         <-- View Model Server Logs
predict-server-pull         <-- Pull Model Server from Docker Registry
predict-server-register     <-- Register Model Server with Docker Registry
predict-server-shell        <-- Shell into Model Server (Debugging)
predict-server-start        <-- Start Model Server
predict-server-stop         <-- Stop Model Server
predict-server-tar          <-- Create Tar File for Model Server
predict-server-tarupload    <-- Tar and Upload Model Server
predict-server-test         <-- Test Model Server (Http-based)
predict-server-untar        <-- Untar Model Server Tar File
predict-server-upload       <-- Upload Model Server Tar File

predict-stream-test         <-- Test Model Server (Stream-based)

stream-http-consume         <-- Consume Stream Messages (REST API)
stream-http-describe        <-- Describe Stream (REST API)
stream-http-produce         <-- Produce Stream Messages (REST API)

stream-kube-consume         <-- Consume Messages from Stream
stream-kube-describe        <-- Describe Stream
stream-kube-produce         <-- Produce Messages to Stream
stream-kube-start           <-- Start Stream (Kafka, MQTT)

train-kube-connect          <-- Create Secure Tunnel to Training Cluster
train-kube-describe         <-- Describe Training Cluster
train-kube-logs             <-- View Training Cluster Logs
train-kube-scale            <-- Scale Training Cluster
train-kube-shell            <-- Shell into Training Cluster
train-kube-start            <-- Start Training Cluster from Docker Registry
train-kube-stop             <-- Stop Training Cluster

train-server-build          <-- Build Training Server
train-server-logs           <-- View Training Server Logs
train-server-pull           <-- Pull Training Server from Docker Registry
train-server-register       <-- Register Training Server with Docker Registry
train-server-shell          <-- Shell into Training Server (Debugging)
train-server-start          <-- Start Training Server
train-server-stop           <-- Stop Training Server

version                     <-- View This CLI Version
```

### 24x7 Support
* Slack:  [![PipelineAI Slack](http://pipeline.ai/assets/img/slack.png)](https://joinslack.pipeline.ai)
* Email:  help@pipeline.ai
* Web:  https://support.pipeline.ai
* Troubleshooting:  [Guide](/docs/troubleshooting)
