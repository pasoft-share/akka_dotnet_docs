---
layout: docs.hbs
title: Akka.NET Documentation
---

## Akka.NET API Docs
- [1.0 Stable API](http://api.getakka.net/docs/stable/index.html)

## Akka.NET Framework
### Introduction
- [What is Akka?](What is Akka.md)
- [Why Akka?](Why Akka.md)
- [Getting Started](Getting started.md)
- [The Obligatory Hello World](The Obligatory Hello World.md)
- Use-case and Deployment Scenarios
	- [Console](deployment-scenarios/Console)
	- [ASP.NET](deployment-scenarios/ASP NET)
	- [Windows Service](deployment-scenarios/Windows Service)
	- [Azure PaaS Worker Role](deployment-scenarios/Azure PaaS Worker Role)
- [Examples of use-cases for Akka](Examples of use cases for Akka.md)

## Akka.NET Concepts
- [Terminology, Concepts](concepts/terminology.md)
- [Actor Systems](concepts/actorsystem.md)
- [What is an Actor?](concepts/actors.md)
- [What is a Message?](concepts/messages.md)
    - [Immutability](concepts/messagesindex.md#messages-are-immutable)
- [Supervision and Monitoring](concepts/supervision.md)
- [Actor References, Paths and Addresses](concepts/addressing.md)
- [Location Transparency](concepts/location-transparency)
- [Message Delivery Reliability](concepts/message-delivery-reliability)
- [Configuration](concepts/configuration.md)
    - [HOCON](concepts/hocon.md)

### Working with Actors
- [Creating your first Actor](working-with-actors/creating-actors)
- [Defining an Actor class](working-with-actors/defining-an-actor)
- [What's in an Actor](working-with-actors/whats-in-an-actor)
- [Creating actors with Props](working-with-actors/creating-actors-with-props)
- [Handling Messages](working-with-actors/handling-messages)
- [Sending Messages](working-with-actors/sending-messages)
- [Actor lifecycle](working-with-actors/Actor lifecycle)
- [Dispatchers](working-with-actors/Dispatchers)
- [Mailboxes](working-with-actors/Mailbox)
- [Switchable Behaviors](working-with-actors/Switchable Behaviors)
- [Stashing Messages](working-with-actors/Stashing Messages)
- [Stopping Actors](working-with-actors/stopping-actors)

### Actors
- [Working with actors](Working with actors.md)
- [F# API](FSharp API.md)
- [ReceiveActors](ReceiveActor.md)
- [Finite State Machines](FSM.md)
- [Persistence](Persistence.md)
- [Fault Tolerance](Fault tolerance.md)
- [Props](Props.md)
- [Receive timeout](Receive timeout.md)
- [Dependency injection](Dependency injection.md)
- [Routers](working-with-actors/Routers)

### Akka.Remote
- [Akka.Remote Overview](remoting/index.md)
    - [Use Cases](remoting/index.md#use-cases)
    - [Enabling Akka.Remote](remoting/index.md#enabling-akka-remote)
    - [Remote Addressing](remoting/index.md#addresses-transports-endpoints-and-associations)
    - [Connecting Remote Systems](remoting/index.md#how-to-form-associations-between-remote-systems)
- [Transports](remoting/transports.md)
    - [Built-in Transports](remoting/transportsindex.md#akka-remote-s-built-in-transports)
    - [Custom Transports](remoting/transportsindex.md#using-custom-transports)
    - [Running Multiple Transports Simultaneously](remoting/transportsindex.md#running-multiple-transports-simultaneously)
- [Remote Messaging](remoting/messaging.md)
    - [Serialization](remoting/messagingindex.md#serialization)
    - [RemoteActorRefs](remoting/messagingindex.md#-remoteactorref-and-location-transparency)
- [Deploying Actors Remotely](remoting/deployment.md)
    - [When to Use Remote Deployment](remoting/deploymentindex.md#when-to-use-remote-deployment)
- [Detecting & Handling Network Failures (DeathWatch)](remoting/deathwatch.md)
- [Network Security](remoting/security.md)

### Akka.Cluster
- [Akka.Cluster Overview](clustering/cluster-overview)
    - [What is a Cluster?](clustering/cluster-overviewindex.md#what-is-a-cluster-)
    - [Benefits](clustering/cluster-overviewindex.md#benefits-of-akka-cluster)
    - [Use Cases](clustering/cluster-overviewindex.md#use-cases)
    - [Terminology](clustering/cluster-overviewindex.md#key-terms)
    - [Enabling Akka.Cluster](clustering/cluster-overviewindex.md#enabling-akka-cluster)
    - [Cluster Gossip](clustering/cluster-overviewindex.md#cluster-gossip)
    - [Nodes](clustering/cluster-overviewindex.md#nodes)
    - [How a Cluster Forms](clustering/cluster-overviewindex.md#how-a-cluster-forms)
- [Cluster Routing](clustering/cluster-routing)
    - [How Routers Use Cluster Gossip](clustering/cluster-routingindex.md#how-routers-use-cluster-gossip)
    - [Cluster Routing Strategies](clustering/cluster-routingindex.md#cluster-routing-strategies)
    - [Types of Clustered Routers](clustering/cluster-routingindex.md#types-of-clustered-routers)
    - [Clustered Router Configuration](clustering/cluster-routingindex.md#cluster-router-config)
- [Cluster Configuration](clustering/cluster-configuration)
    - [Critical Configuration Flags](clustering/cluster-configurationindex.md#critical-configuration-options)
    - [Specifying Minimum Cluster Sizes](clustering/cluster-configurationindex.md#specifying-minimum-cluster-sizes)
- [Accessing the Cluster `ActorSystem` Extension](clustering/cluster-extension)
    - [Getting a Reference to the `Cluster`](clustering/cluster-extensionindex.md#getting-a-reference-to-the-cluster-)
    - [Working With Cluster Gossip](clustering/cluster-extensionindex.md#working-with-cluster-gossip)
    - [Cluster Gossip Event Types](clustering/cluster-extensionindex.md#cluster-gossip-event-types)
    - [Getting Cluster State](clustering/cluster-extensionindex.md#getting-cluster-state)
- [Akka.Cluster.Tools module](clustering/cluster-tools)
    - [Creating cluster singleton actors](clustering/cluster-singleton)
    - [Cluster distributed publish/subscribe](clustering/distributed-publish-subscribe)
    - [Communication with cluster without joining to it](clustering/cluster-client)
- [Akka.Cluster.Sharding module](clustering/cluster-sharding)

### Networking
- [Serialization](Serialization.md)
- [Akka I/O](IO.md)

### Utilities
- [EventBus](EventBus.md)
- [Logging](Logging.md)
  - [Using Serilog](Serilog.md)
- [Scheduler](Scheduler.md)
- [Circuit Breaker](CircuitBreaker.md)

### Testing
- [Using the MultiNode Testkit for Testing Distributed ActorSystems](testing/multinode-testkit)

### Information for Akka Developers
- [Building and Distributing Akka.NET](Building and Distributing Akka.md)
- [Getting Access to Nightly Akka.NET Builds](akka-developers/nightly-builds)
- [Approving Public API Changes](akka-developers/public-api-changes)
- [Contributor guidelines](Contributor guidelines.md)
- [Contribution ideas](Extension Ideas.md)
- [Documentation Guidelines](Documentation guidelines.md)
- [Team](Team.md)

### Project Information
- [Licenses](Licenses.md)
- [Sponsors](Sponsors.md)
- [Project](Project.md)

### Additional Information
- [Frequently Asked Questions](FAQ.md)
- [Community plugins](Community Plugins.md)
- [Online resources](Resources.md)
- [Books](Books.md)
