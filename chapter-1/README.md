# Introducing Kubernetes

**From Monolithic to Microservice**

Before discussing Kubernetes, we need to discuss about the increasing popularity of microservice architecture and container technology. Understanding both phenomenon will give us a proper context on why we need a system like Kubernetes.

In the decade that I became a student in Informatics Engineering and then started my professional career as a software engineer (2000-2010), most software applications I learned to build or I developed for my enterprise clients were developed with monolithic architecture. Scaling were rarely an issue as most of my projects involved only a handful or at most thousands of users.

There are two ways to scale up a software application: vertically (scale up) and horizontally (scale out). To scale up, we just need to add more resources (CPU, RAM, etc) to the machine running our app. As you may guest, there is a low limit on how high we can scale up because there is only limited amount of resources we can add to a single machine. To scale out, we use additional machines to run different copies of the same app. While this alternative is much more scalable than vertical scaling up, this approach may require major change in most monolithic app. For some parts of a monolithic applications, it is even hard or next to impossible to scale out to multiple machines.