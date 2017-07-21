# OpenWIS - Pilots tutorials

This repository hosts a series of mini-tutorials to bring you up to speed to the core concepts and technologies envisaged to be used in future versions of OpenWIS. Each tutorial is composed of a set of slide-like information cards as well as, possibly, source code to demonstrate the concepts. As most tutorials build on the knowledge presented in a previous tutorial, we suggest you start tackling them sequentially.

## OWT-1: Service Oriented Architecture (SOA)
Service-oriented architecture (SOA) is an approach used to create an architecture based upon the use of services. Services carry out some small function, such as producing data, validating a customer, or providing simple analytics. The basic principles of service-oriented architecture are independent of vendors, products and technologies. A service is a discrete unit of functionality that can be accessed remotely and acted upon and updated independently.

According to SOA, a service has the following properties:
- It logically represents a business activity with a specified outcome.
- It is self-contained.
- It is a black box for its consumers.
- It may consist of other underlying services.

Since the definition of SOA does not enforce any technological standards, its implementation can take many forms, such as the following:
- OSGi Services
- ESBs
- REST APIs

This tutorial intends to:
1. Examine the general SOA principles.
2. Illustrate possbile SOA implementations.
3. Discuss SOA best practices.

## OWT-2: SOA using OSGi and Apache Karaf
OSGi (Open Service Gateway Initiative) is a Java framework for developing and deploying modular software programs and libraries. Each bundle is a tightly coupled, dynamically loadable collection of classes, jars, and configuration files that explicitly declare their external dependencies (if any).

Apache Karaf is a small OSGi based runtime that provides a lightweight container onto which various components and applications can be deployed.

This tutorial will cover the following topics:
1. OSGi basics: Bundles & Services.
2. OSGi implementations: Apache Felix, Eclipse Equinox, Knopflerfish, ProSyst.
2. OSGi Karaf features.
4. Deploying bundles on Karaf.

## OWT-3: Creating a service in Karaf
This tutorial will examine the available ways of registering OSGi services (e.g. xml, annotation, etc.) and will provide the first hands-on code example of an OSGi service.

More specifically, it will:
1. Create two bundles.
2. Create two services, one in each bundle.
3. Wire the services together so that communicationis achieved.

## OWT-4: Exposing a service via REST in Karaf using CXF
Apache CXF is an open source services framework that allows developers to build services using frontend programming APIs, like JAX-WS and JAX-RS. These services can speak a variety of protocols such as SOAP, XML/HTTP, RESTful HTTP, or CORBA and work over a variety of transports such as HTTP, JMS or JBI.

This tutorial will integrate CXF into OWT-3 and demonstrate the way to create a REST service using the framework.
The created service will contain 3 methods that will allow a client (e.g. browser) to:
1. Perform a GET request
2. Perform a POST request
3. Receive a response with a custom HTTP status code

## OWT-5: Deploying a web application in Karaf
The purpose of this tutorial is to create the following:
1. A single-page web application
2. A mechanism which will consume the service(s) defined in OWT-4, by using jQuery.

## OWT-6: Deploying an Angular web application in Karaf
Angular is a platform that makes it easy to build applications with the web. It combines declarative templates, dependency injection, end to end tooling, and integrated best practices to solve development challenges. Angular empowers developers to build applications that live on the web, mobile, or the desktop.

This tutorial will create:
1. A single-page web application, much like the one in OWT-5
2. A mechanism which will consume the service(s) defined in OWT-4, built on the Angular framework.

## OWT-7: Database communication in Karaf via services
Hibernate ORM (Hibernate in short) is an object-relational mapping tool for the Java programming language. It provides a framework for mapping an object-oriented domain model to a relational database. Hibernate handles object-relational impedance mismatch problems by replacing direct, persistent database accesses with high-level object handling functions.

The purpose of this tutorial is to showcase database communication in an OSGi service. In particular it will:
1. Enhance the service(s) used in OWT-6, and integrate Hibernate into them.
2. Store and read data from an underlying database.
 
