# ThoughtWorks

## Overview
This project was created on k8s version: v1.19.2

## Build:
Official docker images used:\
    mediawiki: https://hub.docker.com/_/mediawiki \
    mariadb: https://hub.docker.com/_/mariadb

## Deployment
Types of k8s components created:
1. mediawiki-web.yaml (FrontEnd)\
    k8s Deployment\
    k8s service

2. mediawiki-db.yaml (Backend)\
    k8s Deployment\
    k8s service

## Execution steps:
    kubectl apply -f mediawiki-web.yaml
    kubectl apply -f mediawiki-db.yaml


## CI/CD plan
attached .yaml files can be used in the release pipelines (AzureDevops) during the deployment process, and the trigger can be set on master/feature branches of VCS.
