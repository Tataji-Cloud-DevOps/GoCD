# GoCD

### Available Tools for deployments!!!!

    1) Jenkins  ( Jenkins is not really meant for the purpose of deployments, it's main goal is CI )
    2) GoCD     ( This is a contrinuous deployment tool )
    3) ArgoCD   ( This is exclusively for Kubernetes deployments and don't work for server based deployments )

###  CI vs CD vs cd ?  

    CI: Continuous Integration 
    CD: Continuous Deployments vs Continuous Delivery 


### Code Store

    Plain Text code : Git
    Binaries  :  Nexus/artifactory

### Continuous Integration
    
    Continuous Integration is the practice of frequently merging code changes from multiple developers into a shared repository. Each integration triggers an automated build and test process to quickly detect errors. The goal is to catch bugs early, ensure code quality, and keep the codebase in a deployable state.
    
    * Jenkins is a tool that created for this purpose

   Developer---->GIT---->CODE SECURITY CHECK FOR QUALITY(SONACUBE)--->Building artifact(Builds)---->Testing(unit testing,Integration testing,functional testing)---->Tag A release--->Nexus


##  CD (Continuous Delivery / Continuous Deployment):

### CD Tools(Argocd/Gocd)


    Continuous Delivery: Extends CI by ensuring that the code is always in a releasable state. After automated testing, the build is packaged and made ready for deployment to production, but release requires manual approval.

    Continuous Deployment: Goes one step further. Every change that passes automated tests is automatically deployed to production without manual intervention.

    Dev---(will be done only if Dev completed)-->QA---(will be done only if QA completed)-->STAGE---(will be done only if STAGE completed)-->PROD

### GoCD is an open source and FREE

* How GoCD works ---GoCD is a master - node architecture

* Flow

 GoCD server (jobs will be created here)--->Node1(Payment team),Node2(cataloge team)Node3:(cart team)

### GoCD Server requirements: 
    1) t3.small 
    2) 30gb disk 
