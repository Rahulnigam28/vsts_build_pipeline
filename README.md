# Visual Studio Team Services CI/CD Build/Release Pipelines with Azure Container Services (AKS) Workshop

## Overview

This workshop will guide you through building Continuous Integration (CI) and Continuous Deployment (CD) pipelines with Visual Studio Team Services (VSTS) for use with Azure Container Service (AKS - Managed Kubernetes Service).

The labs are based upon a node.js application that allows for voting on the Justice League Superheroes. Data is stored in MongoDB backend.  This builds upon concepts from [Microsoft Intelligent Cloud Blackbelt Team :: Hackfest](https://github.com/Azure/blackbelt-aks-hackfest): Labs 1-3.

The general workflow/result will be as follows:

- Push code to source control (Git hosted in VSTS)
- Trigger a continuous integration (CI) build pipeline when project code is updated via Git
- Package app code into a container image (Docker Image)
- Push docker image to a central container registry (Azure Container Registry) upon a successful build
- Trigger a continuous deployment (CD) release pipeline upon a successful build
- Deploy container image to target deployment environment/platform (Azure Container Services aka. ACS or AKS) upon successful a release
- Rinse and repeat upon each code update via Git
- Profit

![workflow](hol-content/img/workflow.png)


## Prerequisite Lab

[Microsoft Intelligent Cloud Blackbelt Team :: Hackfest](https://github.com/Azure/blackbelt-aks-hackfest): Labs 1-5
  - This HoL/hackfest is a detailed guide to deploying apps to a Kuberenetes istributed computing cluster on Azure (i.e. AKS)


## Hands-on Lab Guide

1. [Setting up VSTS](hol-content/01-setup_vsts.md)
2. [Building a VSTS Continuous Integration Pipeline](hol-content/02-build_vsts_ci.md)
3. [Building a VSTS Continuous Deployment Pipeline](hol-content/03-build_vsts_cd.md)

## Maintainers and Contact Information

- Kevin Harris - [@kevingbb](https://github.com/kevingbb)
- Ray Kao - [@raykao](https://github.com/raykao)
