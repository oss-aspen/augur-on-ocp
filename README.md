# Augur on OpenShift

This repository contains the necessary files to deploy Augur on OpenShift. It
is organized around Kustomize and ArgoCD.


## Setup

Cluster needs the following operators installed:

https://github.com/CrunchyData/postgres-operator


https://github.com/rabbitmq/cluster-operator

## Usage

1. copy `deploy/augur-secret-example.yml` to `deploy/augur-secret.yml`and edit the values

2. deploy using `oc apply -k deploy`

3. configure any routes you desire for services you want externally accessible.
