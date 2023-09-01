
This repository is a continuation of the CI pipeline described in the repo: https://github.com/marcusmvbs/SRE-gitlab-CI-Proj-2. ArgoCD utilized to deploy updates on manifest files, that configures a kubernetes cluster on Google cloud. This separation was intended to adopt gitops practices, for a CI/CD pipeline. 

Kubernetes is being used to deploy several services as: 
    Nginx ingress controller;
    Nginx server;
    Redis for caching content;
    Kasten k10 - backup;
    Fluent bit - logs;
    Prometheus - monitoring;
    Postgresql database - to write on a persistent volume on google cloud.

The project was created for study purposes. Improvements on config maps and secrets for each namespace, better configuration of each service described in the diagram, are still a work in progress. 