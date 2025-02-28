---
title: Distributed Apps
status: Feedback Appreciated
category: concept
---
## Distributed Apps

### What it is

A distributed application is an application where the functionality is broken down into multiple smaller independent parts. Distributed applications are usually composed of individual [microservices](https://github.com/cncf/glossary/blob/main/definitions/microservices.md) that handle different concerns within the broader application. In a cloud native environment the individual components typically run as [containers](https://github.com/cncf/glossary/blob/main/definitions/container.md) on a [cluster](https://github.com/cncf/glossary/blob/main/definitions/cluster.md). 

### The problem it addresses 

An application running on one single computer represents a single point of failure — if that computer fails, the application becomes unavailable. Distributed applications are often contrasted to monolithic applications. A monolithic app can be harder to scale as the various components can't be scaled independantly. They can also become a drag on developer velocity as they grow because more developers need to work on a shared codebase that doesn't necessarily have well defined boundaries.

### How it helps

When splitting an application into different pieces and running them in many places, the overall system can tolerate more failures. It also allows an application to take advantage of scaling features not available to a single application instance, namely the ability to [scale horizontally](https://github.com/cncf/glossary/blob/main/definitions/horizontal-scaling.md). This does, however, come at a cost: increased complexity and operational overhead — you’re now running lots of application components instead of one app.

