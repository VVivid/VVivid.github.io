---
title: "Introduction to Microservices Series"
date: 2022-03-23T01:56:28+07:00
slug: ""
description: "Understanding of microservice architecture "
keywords: ["k8s"]
draft: false
tags: ["microservices"]
math: false
toc: false
---

If you have follow the tech trend recently you will most likely to encounter the word Microservice and hundreds of blogs are talking about how powerful it is that it's starting to sound like a magical hack in the software development world. This blog is no different to the other blogs out there, but beside learning about what microservice is in this series we will also looking into other technologies and concepts that help us build a truly maintainable and scalable microservices architecture.

## What really is a Microservice?<br>

If I could over simplify the meaning of Microservice is that microservice is the way you split all your business logic or the requirements to support your business into multiple services and run it separately either by the same team or multiple team working on different service.

![microservice architecture](/svg/architecture.png)

## Why would you consider using a Microservice architecture?<br>

Microservice has it name because of its ability to improve them system scalability and its give more freedom to the development teams to work on various kind of technologies that they are comfortable with and the teams can focus on their expertise and scale the services independently without have to worry of slowing down another team.

## Should you start with Microservice from the beginning?<br>

The answer is not really because most of the time the system still be working fine running as Monolith, and instead you should always start with a monolith application at first and then try to optimize your application performance until at some points you will starting to see a unique growth on only some part of your system and that is when you know which service should be splitting.

## Is there any disadvantages using Microservices?<br>

yes, and there are many disadvantages as well. One of the biggest issue is latency, as you need to split your services there will be time where in order to complete a simple task it would requires 2 or 3 services to do it and unlike monolith application these services have to agree on some type of communication and usually requires additional network latency from one service to another.

![latency](/svg/latency.png)

The second one is complexity, so when you have a lot of services running it will be hard for you to manage and monitoring all your services, and sometime a single service update could effect other services that depend on it, so you will need a better tooling for that. The last one is development team size has to grow in other to manages all of those services.

For this series we will have a peak into most commonly use communication technique between services like gRPC, Messaging Queue and event base communication. We will also looking into container technologies like Docker and how we could use it to deploy our microservices and to advance where Kubernetes come into be more useful when we have a lots of services and deploying starting to get more difficult and hard to manage. Also we will start learning more about some infrastructure tools like proxy, load balance and API gateway to secure and isolate our services. Finally, we will also look into some other tools for logging and debugging like Loki, Promtail and Grafana to push to our log system and visualize it on Grafana dashboard.

Lastly, I want to clarify that I'm no expert in all of these, however this is just a part of my experience as a software engineer and this series is where I documented what I have learn during those time. I hope you find this helpful and enjoy it.

