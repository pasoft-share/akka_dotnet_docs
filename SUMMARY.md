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
	- [Console](deployment-scenarios/Console.md)
	- [ASP.NET](deployment-scenarios/ASP NET.md)
	- [Windows Service](deployment-scenarios/Windows Service.md)
	- [Azure PaaS Worker Role](deployment-scenarios/Azure PaaS Worker Role.md)
- [Examples of use-cases for Akka](Examples of use cases for Akka.md)

## Akka.NET Concepts
- [Terminology, Concepts](concepts/terminology.md)
- [Actor Systems](concepts/actorsystem.md)
- [What is an Actor?](concepts/actors.md)
- [What is a Message?](concepts/messages.md)
    - [Immutability](concepts/messages#messages-are-immutable)
- [Supervision and Monitoring](concepts/supervision.md)
- [Actor References, Paths and Addresses](concepts/addressing.md)
- [Location Transparency](concepts/location-transparency.md)
- [Message Delivery Reliability](concepts/message-delivery-reliability.md)
- [Configuration](concepts/configuration.md)
    - [HOCON](concepts/hocon.md)

### Working with Actors
- [Creating your first Actor](working-with-actors/creating-actors.md)
- [Defining an Actor class](working-with-actors/defining-an-actor.md)
- [What's in an Actor](working-with-actors/whats-in-an-actor.md)
- [Creating actors with Props](working-with-actors/creating-actors-with-props.md)
- [Handling Messages](working-with-actors/handling-messages.md)
- [Sending Messages](working-with-actors/sending-messages.md)
- [Actor lifecycle](working-with-actors/Actor lifecycle.md)
- [Dispatchers](working-with-actors/Dispatchers.md)
- [Mailboxes](working-with-actors/Mailbox.md)
- [Switchable Behaviors](working-with-actors/Switchable Behaviors.md)
- [Stashing Messages](working-with-actors/Stashing Messages.md)
- [Stopping Actors](working-with-actors/stopping-actors.md)

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
- [Routers](working-with-actors/Routers.md)

### Akka.Remote
- [Akka.Remote Overview](remoting/index.md)
    - [Use Cases](remoting/#use-cases)
    - [Enabling Akka.Remote](remoting/#enabling-akka-remote)
    - [Remote Addressing](remoting/#addresses-transports-endpoints-and-associations)
    - [Connecting Remote Systems](remoting/#how-to-form-associations-between-remote-systems)
- [Transports](remoting/transports.md)
    - [Built-in Transports](remoting/transports#akka-remote-s-built-in-transports)
    - [Custom Transports](remoting/transports#using-custom-transports)
    - [Running Multiple Transports Simultaneously](remoting/transports#running-multiple-transports-simultaneously)
- [Remote Messaging](remoting/messaging.md)
    - [Serialization](remoting/messaging#serialization)
    - [RemoteActorRefs](remoting/messaging#-remoteactorref-and-location-transparency)
- [Deploying Actors Remotely](remoting/deployment.md)
    - [When to Use Remote Deployment](remoting/deployment#when-to-use-remote-deployment)
- [Detecting & Handling Network Failures (DeathWatch)](remoting/deathwatch.md)
- [Network Security](remoting/security.md)

### Akka.Cluster
- [Akka.Cluster Overview](clustering/cluster-overview.md)
    - [What is a Cluster?](clustering/cluster-overview#what-is-a-cluster-)
    - [Benefits](clustering/cluster-overview#benefits-of-akka-cluster)
    - [Use Cases](clustering/cluster-overview#use-cases)
    - [Terminology](clustering/cluster-overview#key-terms)
    - [Enabling Akka.Cluster](clustering/cluster-overview#enabling-akka-cluster)
    - [Cluster Gossip](clustering/cluster-overview#cluster-gossip)
    - [Nodes](clustering/cluster-overview#nodes)
    - [How a Cluster Forms](clustering/cluster-overview#how-a-cluster-forms)
- [Cluster Routing](clustering/cluster-routing.md)
    - [How Routers Use Cluster Gossip](clustering/cluster-routing#how-routers-use-cluster-gossip)
    - [Cluster Routing Strategies](clustering/cluster-routing#cluster-routing-strategies)
    - [Types of Clustered Routers](clustering/cluster-routing#types-of-clustered-routers)
    - [Clustered Router Configuration](clustering/cluster-routing#cluster-router-config)
- [Cluster Configuration](clustering/cluster-configuration.md)
    - [Critical Configuration Flags](clustering/cluster-configuration#critical-configuration-options)
    - [Specifying Minimum Cluster Sizes](clustering/cluster-configuration#specifying-minimum-cluster-sizes)
- [Accessing the Cluster `ActorSystem` Extension](clustering/cluster-extension.md)
    - [Getting a Reference to the `Cluster`](clustering/cluster-extension#getting-a-reference-to-the-cluster-)
    - [Working With Cluster Gossip](clustering/cluster-extension#working-with-cluster-gossip)
    - [Cluster Gossip Event Types](clustering/cluster-extension#cluster-gossip-event-types)
    - [Getting Cluster State](clustering/cluster-extension#getting-cluster-state)
- [Akka.Cluster.Tools module](clustering/cluster-tools.md)
    - [Creating cluster singleton actors](clustering/cluster-singleton.md)
    - [Cluster distributed publish/subscribe](clustering/distributed-publish-subscribe.md)
    - [Communication with cluster without joining to it](clustering/cluster-client.md)
- [Akka.Cluster.Sharding module](clustering/cluster-sharding.md)

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
- [Using the MultiNode Testkit for Testing Distributed ActorSystems](testing/multinode-testkit.md)

### Information for Akka Developers
- [Building and Distributing Akka.NET](Building and Distributing Akka.md)
- [Getting Access to Nightly Akka.NET Builds](akka-developers/nightly-builds.md)
- [Approving Public API Changes](akka-developers/public-api-changes.md)
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
