# Awesome AMQP 1.0 [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
A curated list of AMQP 1.0 resources. Unless explicitly stated, AMQP in this list refers to AMQP 1.0.

> The Advanced Message Queuing Protocol (AMQP) is the Internet Protocol for Business Messaging. It is designed to be secure, reliable, interoperable, standard and open.

## Table of Contents

- [Protocol Specifications](#protocol-specifications)
- [Introduction](#introduction)
- [Brokers](#brokers)
- [Routers, Adapters, Bridges](#routers-adapters-bridges)
- [Libraries and Clients](#libraries-and-clients)
- [Tools](#tools)
- [More Reading](#more-reading)
- [Contribute](#contribute)


### Protocol Specifications

**Core Protocol**
* [OASIS Advanced Message Queuing Protocol (AMQP)](http://docs.oasis-open.org/amqp/core/v1.0/os/amqp-core-overview-v1.0-os.xml).

**Extended Specifications and Bindings**
* [AMQP WebSockets Binding](http://docs.oasis-open.org/amqp-bindmap/amqp-wsb/v1.0/amqp-wsb-v1.0.html) - Defines using the WebSocket protocol as a transport for AMQP (Committee Specification 01).
* [AMQP Addressing](https://www.oasis-open.org/committees/download.php/52063/amqp-addressing-v1.0-wd05.pdf) - Defines a standard text based syntax and semantics for message addresses used with AMQP (working draft).
* [AMQP Management Specification](https://www.oasis-open.org/committees/document.php?document_id=54441&wg_abbrev=amqp) - Defines a request/response protocol over AMQP to perform management operations (working draft).
* [AMQP Claims-based Security](https://www.oasis-open.org/committees/document.php?document_id=50506&wg_abbrev=amqp) - Defines a layered protocol to authenticate AMQP clients using security tokens (working draft).
* [AMQP JMS Mapping](https://www.oasis-open.org/committees/download.php/60251/amqp-bindmap-jms-v1.0-wd08.pdf) - Defines a mapping for supporting JMS using AMQP as the wire protocol (working draft).

**OASIS AMQP Technical Committee**
* [OASIS AMQP TC](https://www.oasis-open.org/committees/tc_home.php?wg_abbrev=amqp) - Information about the AMQP Technical Committee.


### Introduction

* [amqp.org](http://www.amqp.org/) - The web site.
* [Clemens Vasters Channel9 Subscribe!](https://channel9.msdn.com/Blogs/Subscribe) - A series of videos explaining the core components in AMQP.
  * [Overview](https://channel9.msdn.com/Blogs/Subscribe/The-AMQP-10-Protocol-16-Overview).
  * [Core Elements](https://channel9.msdn.com/Blogs/Subscribe/The-AMQP-10-Protocol-26-Core-Elements).
  * [Message Transfers](https://channel9.msdn.com/Blogs/Subscribe/The-AMQP-10-Protocol-36-Message-Transfers).
  * [Flow Control](https://channel9.msdn.com/Blogs/Subscribe/The-AMQP-10-Protocol-46-Flow-Control).
  * [Primitive Type Encoding](https://channel9.msdn.com/Blogs/Subscribe/The-AMQP-10-Protocol-56-Primitive-Type-Encoding).
  * [Composite Types and Messages](https://channel9.msdn.com/Blogs/Subscribe/The-AMQP-10-Protocol-66-Composite-Types-and-Messages).
  * [YouTube Playlist](https://www.youtube.com/watch?v=ODpeIdUdClc&list=PLmE4bZU0qx-wAP02i0I7PJWvDWoCytEjD).
* [Apache Qpid](https://qpid.apache.org/) - Messaging built on AMQP 1.0.
* [AMQP Essentials](https://dzone.com/refcardz/amqp-essentials) by Paolo Patierno. Practical introduction to AMQP.


### Brokers

* [Microsoft Azure Service Bus](https://azure.microsoft.com/en-us/services/service-bus/) - Cloud Messaging (queues, pub/sub).
* [Microsoft Azure Event Hubs](https://azure.microsoft.com/en-us/services/event-hubs/) - Cloud-scale telemetry service.
* [Microsoft Service Bus For Windows Server (Service Bus 1.1)](https://msdn.microsoft.com/en-us/library/dn282144.aspx).
* [Apache ActiveMQ](http://activemq.apache.org/) - An open source message broker written in Java. AMQP is one of the supported protocols.
* [Apache ActiveMQ Apollo](http://activemq.apache.org/apollo/) - ActiveMQ's next generation of messaging.
* [Apache ActiveMQ Artemis](http://activemq.apache.org/artemis/) - An attempt to merge a number of ActiveMQ features with HornetQ.
* [Apache Qpid Java Broker](http://qpid.apache.org/components/java-broker/) - A pure-Java AMQP message broker.
* [Apache Qpid C++ Broker](http://qpid.apache.org/components/cpp-broker/index.html) - A native-code AMQP message broker.
* [Red Hat JBoss A-MQ](https://www.redhat.com/en/technologies/jboss-middleware/amq) - Based on Apache ActiveMQ.
* [SwiftMQ](http://www.swiftmq.com) - A JMS broker that has AMQP 1.0 support.
* [IBM MQ with AMQP channel](https://www.ibm.com/support/knowledgecenter/SSFKSJ_8.0.0/com.ibm.mq.amqp.doc/amqp_support.htm).
* [RabbitMQ with AMQP 1.0 plugin](https://www.rabbitmq.com/plugins.html) - [Experimental](https://github.com/rabbitmq/rabbitmq-amqp1.0).


### Routers, Adapters, Bridges

* [Apache Qpid Dispatch Router](http://qpid.apache.org/components/dispatch-router/index.html) - An AMQP router for scalable messaging interconnect.
* [SwiftMQ AMQP Router](http://www.swiftmq.com/products/amqprouter/index.html).
* [Sqlstream AMQP adapter](http://sqlstream.com/docs/int_amqpadapter.html).
  * [Write](http://sqlstream.com/docs/int_ecda_writing_amqp.html) to AMQP destination.
  * [Read](http://sqlstream.com/docs/int_ecda_reading_amqp.html) from AMQP source.
* [OpenMAMA AMQP Bridge](http://www.openmama.org/middleware-bridges) - Enable communication over AMQP through the Middleware Agnostic Messaging API.
* [AMQP - Apache Kafka bridge](https://github.com/rhiot/amqp-kafka-bridge) - Connect AMQP clients to Apache Kafka cluster.
* [AMQP - Apache Spark Streaming](https://github.com/radanalyticsio/streaming-amqp) - Connect AMQP clients to Apache Spark cluster on the streaming side.


### Libraries and Clients

* [Microsoft AmqpNetLite](https://github.com/Azure/amqpnetlite) - C#.
* [Microsoft AmqpNetMicro](https://www.nuget.org/packages/AMQPNetMicro/) - A compact version of AmqpNetLite for .Net Micro Framework.
* [Microsoft Azure AMQP](https://github.com/Azure/azure-amqp) - C#.
* [Microsoft uAMQP](https://github.com/azure/azure-uamqp-c/) - C.
* [Apache Qpid JMS](https://qpid.apache.org/components/jms/) - AMQP 1.0 JMS client.
* [Apache Qpid Proton](https://qpid.apache.org/proton/index.html) - The AMQP messaging toolkit in various languages.
  * Proton-C: C and its language bindings (cpp, go, javascript, node, perl, php, python and ruby).
  * Proton-J: Java.
* [node-amqp10](https://github.com/noodlefrenzy/node-amqp10) - A promise-based, AMQP 1.0 compliant node.js client.
* [Rhea](https://github.com/grs/rhea) - A node.js client.
* [SwiftMQ AMQP 1.0 Client](http://www.swiftmq.com/products/client/index.html) - Java.
* [IBM MQ Light](https://developer.ibm.com/messaging/mq-light/) - AMQP 1.0 clients for node.js, Java, Ruby, Python.
* [amqp-io](https://github.com/xinchen10/amqp-io) - An AMQP serializer for Java objects.
* [vertx-amqp-bridge](https://github.com/vert-x3/vertx-amqp-bridge) - AMQP 1.0 support implementing the Vert.x MessageProducer and MessageConsumer APIs over vertx-proton.
* [vertx-proton](https://github.com/vert-x3/vertx-proton) - A thin Vert.x integration for the Apache Qpid Proton protocol engine.
* [Rhea Node](https://github.com/ppatierno/rhea-node) - AMQP 1.0 nodes for [Node-RED](http://nodered.org/) and flow programming.


### Tools

* [AMQP 1.0 interactive type reference](http://qpid.apache.org/amqp/type-reference.html).
* [Adverb](https://github.com/ChugR/Adverb) - Distill AMQP net trace into web page.
* [Wireshark with AMQP 1.0 dissector](https://www.wireshark.org/).
* [SwiftMQ AMQP 1.0 Test Suite](http://www.swiftmq.com/developers/amqp_testsuite/index.html).
* [TestAmqpBroker from AMQP.Net Lite](https://github.com/Azure/amqpnetlite/tree/master/test/TestAmqpBroker).


### More Reading

* [Clarifying AMQP](http://kellabyte.com/2012/10/20/clarifying-amqp/) by Kelly Sommers. How the AMQP 1.0 protocol is completely different from the old AMQP 0.9 protocol.
* [Hello World!](https://chugrolke.wordpress.com/2015/08/03/hello-world/) by Chuck Rolke. AMQP.Net Lite client connecting to [Red Hat JBoss A-MQ broker](https://access.redhat.com/documentation/en-US/Red_Hat_JBoss_A-MQ/6.2/index.html).
* [AMQP Illustrated](https://chugrolke.wordpress.com/2015/08/27/amqp-illustrated/) by Chuck Rolke. Code walkthrough of the Hello World! example and Wireshark capture of network traces.
* [AMQP protocol built in type system by example](https://paolopatierno.wordpress.com/2015/07/20/amqp-protocol-the-builtin-type-system-by-examples/) by Paolo Patierno. Introduction to AMQP frames and built in type system.
* [AMQP on the wire messages content framing](https://paolopatierno.wordpress.com/2015/07/23/amqp-on-the-wire-messages-content-framing/) by Paolo Patierno. A journey inside the messages structure with a sending example.
* [AMQP message accepted encoding on the wire](https://paolopatierno.wordpress.com/2015/07/24/amqp-message-accepted-encoding-on-the-wire/) by Paolo Patierno. What it means to receive and accept a message at wire level.
* [Routing AMQP : The Qpid Dispatch Router project](https://paolopatierno.wordpress.com/2016/03/21/routing-amqp-the-qpid-dispatch-router-project/) by Paolo Patierno. Introduction to the AMQP router project.
* [Qpid Dispatch Router installation on your Linux machine](https://paolopatierno.wordpress.com/2016/04/25/qpid-dispatch-router-installation-on-your-linux-machine/) by Paolo Patierno. Installing the AMQP router on a Linux machine.
* [Routing mechanisms for AMQP protocol](https://paolopatierno.wordpress.com/2016/05/10/routing-mechanisms-for-amqp-protocol/) by Paolo Patierno. AMQP routing mechanisms available with the AMQP router.
* [My Raspberry Pi runs the Qpid Dispatch Router](https://paolopatierno.wordpress.com/2016/05/14/my-raspberry-pi-runs-the-qpid-dispatch-router/) by Paolo Patierno. How to run the AMQP router on a Raspberry Pi.
* [A routing IoT gateway to the Cloud](https://paolopatierno.wordpress.com/2016/07/23/a-routing-iot-gateway-to-the-cloud/) by Paolo Patierno. How to use the AMQP router as field IoT gateway to the Azure IoT Hub.
* [Differences between AMQP 0-10 and AMQP 1.0](https://access.redhat.com/documentation/en-US/Red_Hat_Enterprise_MRG/3/html/Messaging_Programming_Reference/Differences_between_AMQP_0-10_and_AMQP_1.0.html).
* [What's up with AMQP 1.0?](http://blogs.mulesoft.com/dev/mule-dev/whats-up-with-amqp-1-0/).


### Presentations

* [Azure Service Bus : under the hood](http://www.slideshare.net/paolopat/azure-service-bus-under-the-hood) by Paolo Patierno. How the AMQP protocol works under the cover of the Azure Service Bus.
* [IoT protocols war ! Battles on the fields ...](http://www.slideshare.net/paolopat/internet-ofthingsprotocolswar) by Paolo Patierno. Comparison between AMQP, MQTT, HTTP and CoAP on different fields like : architecture, implementation and weight, data transport and manipulation, IoT communication patterns and security.
* [IoT protocols landscape](http://www.slideshare.net/paolopat/io-t-protocols-landscape) by Paolo Patierno. Comparison between AMQP, MQTT, HTTP and CoAP on all their provided features.


### Contribute

Contributions welcome! Read the [contribution guidelines](CONTRIBUTING.md) first.


## License

[![CC0](http://i.creativecommons.org/p/zero/1.0/88x31.png)](http://creativecommons.org/publicdomain/zero/1.0/)
