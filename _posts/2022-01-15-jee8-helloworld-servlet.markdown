---
layout: post
title:  "Creating a JEE 8 Hello World Servlet Maven Archetype in Eclipse 2021"
date:   2021-12-26 11:57:21 -0400
categories: software engineering entrepreneur
---

#### Overview

The latest version of Eclipse now requires JDK 11, and it is enabled for JEE 8 Platform Edition

We want to create a Maven Archetype of a JEE 8 Servlet Application using this latest version of Eclipse
[What is a Maven Archetype?](https://maven.apache.org/archetype/index.html)

The reason we want to do this is that not all our developers and distributed teams use Eclipse, and we want to have
everyone in the organization use our approved Java Project structure

#### High Level Steps 

1. Create an Eclipse Web App using the Eclipse Wizard
2. Create a Maven War App using the Maven War Archetype
3. Use the Eclipse projects created in step 1 and step 2 to create our JEE 8 Hello World Servlet Archetype
4. Generate an example JEE 8 Hello World Servlet project in Eclipse using our very own Archetype

#### [Guide to Creating Archetypes](https://maven.apache.org/guides/mini/guide-creating-archetypes.html)

#### Creating the Eclipse Java Web App

- Select Java Web App New Project Wizard
- Select version 4.0 which is compliant with JEE 8
- Generate web descriptor web.xml
- Add Java Servlet Code and Configuration entry
- Run and test the Web App

#### Create a Maven War App using the Maven War Archetype 

- File New Maven Project
- Select maven-webapp-archetype version 1.4
- Package com.nicordesigns Group Id HelloWorldServlet
- Fix JSP Problem by adding the required Jakarta Servlet Package Dependency in Maven POM
- Update POM to Java 1.8 (required for JEE 8)
- Repeat all the updates done for the Eclipse project
- Run and test the web app

#### Use our Maven JEE8 Hello World Servlet App to create a new Archetype

- mvn archetype:create-from-project
- make sure the generated archetype is correct and requires everything we need
- generate a test project from our new archetype
- run our new test project

If you'd like to support my channel, you can donate via PayPal: [Donate via PayPal](https://paypal.me/nicordesigns?country.x=US&locale.x=en_US)

[![SOAP-WS YOUTUBE TUTORIAL](https://img.youtube.com/vi/d6rAG11goFM/mq2.jpg)](https://www.youtube.com/watch?v=d6rAG11goFM)


