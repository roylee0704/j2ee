# Java Web Application (Module)

## Introduction

In-short, this module is responsible for Web (Front) development, which includes:

1. JSP
2. HTML & JS & CSS
2. /WEB-INF/web.xml

## JSP (Java Server Pages) 

A combinationation of both Java (<%scriplets%>) + HTML. Upon receiving HTTP request from client, Server dissect/locate/compile the respective JSP
into `Servlets` and then stream back to client browser. 

Its output stream can in various format:
- HTML document.
- PDF document.
- Image file. (jpg, gif, png, etc) 

## HTML & JS & CSS

Basically, these are the web technogies that powers the front-end user experiences. 

## /WEB-INF/web.xml

This file serves as the interface layer between `EJB/SessionBean(@local)` by exposing Java API interface to be called by `JSP`.

In XML format, it contains the following information:
- Unique file name.
- Mapping information between *EJB/SessionBean classpath* and *reference name* to be used in `JSP`.

To call in `JSP`.
```java
	ctx.lookup("<reference name of EJB classpath>");
```

## Artifact

An artifact also known as the output of particular Java module. In Java Web Application, it has the format of `*.WAR`.



//todo:
- xml content
- improve jsp lookup example
- how to add ejb session bean's classpath in web.xml.


