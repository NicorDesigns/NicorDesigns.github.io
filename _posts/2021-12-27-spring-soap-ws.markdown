---
layout: post
title:  "Beginners Introduction to SOAP with SPRING-WS"
date:   2021-12-27 11:57:21 -0400
categories: software engineering entrepreneur
---

#### SOAP with SPRING-WS

How to implement SOAP Web Services with Spring Web Services?
How to use a free third party tool SOAP-UI to test our SOAP Web Service?

#### UNDERSTANDING SOAP

SOAP is a protocol designed to exchange information. It is primarily based on XML documents over HTTP,  but email and 
JMS can also be used.

SOAP web services are based on a Web Services Description Language, WSDL, which is an XML contract that defines all the 
data and services offered by a given web service.

The client and the server both use this contract as a basis for exchanging information and making remote procedural 
calls.

#### [SOAP Specification](https://www.w3.org/TR/soap/)

#### Introduction to SOAP with SPRING-WS

- Spring-WS is a product of the Spring community for SOAP Web services.

- Spring Web Services aims to facilitate contract-first SOAP service development

- The product is based on Spring itself.

- People use Spring-WS after finding alternative SOAP stacks lacking

- Best Practise: Contract-First development, and having a loose coupling between contract and implementation.

#### SPRING-WS SOAP Reference Manual
[http://spring.io/projects/spring-ws#overview](http://spring.io/projects/spring-ws#overview)

[http://spring.io/projects/spring-ws#learn](http://spring.io/projects/spring-ws#learn)

[https://spring.io/understanding/SOAP](https://spring.io/understanding/SOAP)

#### What we will learn

- SOAP Prerequisite concepts XML, XSD, WSDL

- We will create a SOAP Endpoint with Spring-WS

- We will install a SOAP client test tool SOAP-UI

#### Business Problem

Build a SOAP Service that accept Insurance Contracts for Widgets

Widget co is screaming for the WSDL!
The client is going to send us an XML document over HTTP.
This XML document will conform to a SOAP envelope specification.
Our SOAP service will accept this XML Insurance Application Document and return an acknowledge receipt document in XML 
format that will conform to the SOAP specification.
Now, all of this will be specified in our WSDL document.
Which means once the WSDL is published the client Widget Co will know what they will have to send to us and what XML 
document they will receive in acknowledgment.

#### Questions

1. How will we create and expose our SOAP endpoint?
2. How will the client connect with our SOAP endpoint?
3. What language will the client use?

#### Answers

1. We will  use Spring-WS to define our SOAP Endpoint,  Spring-WS will generate the WSDL for us, the client will access 
the WSDL from a public URL
2. The client will connect with SOAP over HTTP
3. The client can use any language such as C#, COBOL to interact with our exposed SOAP Web Service. 

The client has to use:

[![SOAP-WS YOUTUBE TUTORIAL](https://img.youtube.com/vi/d6rAG11goFM/mq2.jpg)](https://www.youtube.com/watch?v=d6rAG11goFM)


