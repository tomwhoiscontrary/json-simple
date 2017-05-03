JSON.simple - A simple Java toolkit for JSON

# GitHub

https://github.com/fangyidong/json-simple

# Overview

JSON.simple is a simple Java toolkit for JSON. You can use JSON.simple to encode or decode JSON text.

# Features

* Full compliance with [JSON specification](http://www.ietf.org/rfc/rfc4627.txt) (RFC4627) and reliable (see compliance testing)
* Provides multiple functionalities such as encode, decode/parse and escape JSON text while keeping the library lightweight
* Flexible, simple and easy to use by reusing Map and List interfaces
* Supports streaming output of JSON text
* Stoppable SAX-like interface for streaming input of JSON text (learn more)
* Heap based parser
* High performance (see performance testing)
* No dependency on external libraries
* Both of the source code and the binary are JDK1.2 compatible

# Getting Started

Note: You need to put the latest [json-simple-1.1.1.jar](http://repo1.maven.org/maven2/com/googlecode/json-simple/json-simple/1.1.1/json-simple-1.1.1.jar) in your CLASSPATH before compiling and running the example codes.

* Encoding Examples
* Decoding Examples
* Escaping Examples
* JSP and AJAX Examples

# Mapping Between JSON and Java Entities

| JSON       | Java              |
| :--------- | :---------------- |
| string     | java.lang.String  |
| number     | java.lang.Number  |
| true|false | java.lang.Boolean |
| null       | null              |
| array      | java.util.List    |
| object     | java.util.Map     |

JSON.simple maps entities from the left side to the right side while decoding or parsing, and maps entities from the right to the left while encoding. While decoding, default concrete class of java.util.List is org.json.simple.JSONArray and default concrete class of java.util.Map is org.json.simple.JSONObject. While encoding, other classes that are not listed on the right side of the table need to implement JSONAware or JSONStreamAware (streaming only) to [customize](EncodingExamples.md) JSON outputs. In such cases, JSON.simple calls JSONAware.toJSONString() or JSONStreamAware.writeJSONString() to determine the resulting JSON text.

# Maven Repository

* JSON.simple in central maven repository

# Developer's Guide

* Build With Ant
* Build With Eclipse
* The JSON Lexer

# JSON.simple in Projects/Products

* [Vuze (Azureus)](http://azureus.sourceforge.net/)
* [Apache Cassandra](http://incubator.apache.org/cassandra/)
* [Apache Clerezza](http://incubator.apache.org/clerezza/)
* [Apache MyFaces](http://myfaces.apache.org/)
* [Apache Oozie(TM) Workflow Scheduler for Hadoop](http://incubator.apache.org/oozie/)
* [Apusic OperaMasks](http://www.operamasks.org)
* [Chartle.net](http://www.chartle.net/)
* [co-ode-owl-plugins](http://code.google.com/p/co-ode-owl-plugins/)
* [google-caja](http://code.google.com/p/google-caja/)
* [Google Chrome Developer Tools for Java](http://code.google.com/p/chromedevtools/)
* [GV](http://www.evancharlton.com/projects/gv)
* [Hula from Novell](http://developer.novell.com/wiki/index.php/Hula)
* [jmx4perl](http://search.cpan.org/~roland/jmx4perl/lib/JMX/Jmx4Perl/Manual.pod)
* [Json2Ldap](http://software.dzhuvinov.com/ldap-gateway.html)
* [Kindle3](http://www.amazon.com/Kindle-Wireless-Reader-Wifi-Graphite/dp/B002Y27P3M)
* [LabKey Server](http://www.labkey.com/)
* [Log4Ant](http://jwaresoftware.org/wiki/log4ant/home)
* [Mozilla Bespin](https://bespin.mozilla.com/)
* [MTS](http://chcr.umich.edu/mts/)
* [MUSCLE](http://muscle.berlios.de/)
* [NoiseTube](http://www.noisetube.net/)
* [NuGram Platform](http://nugram.nuecho.com/welcome)
* [PhyloWidget](http://www.phylowidget.org/)
* [Renren.com Open API](http://wiki.dev.renren.com/wiki/%E5%9C%A8%E4%BD%A0%E7%9A%84Web%E5%BA%94%E7%94%A8%E4%B8%AD%E6%98%BE%E7%A4%BA%E7%94%A8%E6%88%B7%E5%A7%93%E5%90%8D%E5%92%8C%E5%A4%B4%E5%83%8F)
* [Sonar](http://www.sonarsource.org/)
* [Teiid](http://www.jboss.org/teiid)
* [Twitter elephant-bird](https://github.com/kevinweil/elephant-bird)
* [TopQuadrant TopBraid Suite™](http://www.topquadrant.com/products/TB_Suite.html)
* [vtiger CRM Web Services Client Library](http://forge.vtiger.com/projects/vtwsclib)
* [XBrain](http://sig.biostr.washington.edu/projects/xbrain/)
* [ZK.forge](http://sourceforge.net/projects/zkforge/)

# JSON.simple in Fedora

* [Fedora 12, Fedora 11 and Fedora EPEL 5](https://admin.fedoraproject.org/pkgdb/packages/name/json_simple)

# JSON.simple in Ubuntu

* [Ubuntu Oneiric](http://packages.ubuntu.com/oneiric/libjson-simple-java)

# JSON.simple in Publications

* [O'Reilly - Ajax On Java](http://oreilly.com/catalog/9780596101879/)
* [Ajax development case study](http://www.tup.tsinghua.edu.cn/book/SHOWBOOK.asp?cpbh=025070-01)
* [Tutorial from webucator](http://www.webucator.com/WebDesign/JSC401.cfm)
* [A Review of 5 Java JSON Libraries (Rob@Rojotek)](http://www.rojotek.com/blog/2009/05/07/a-review-of-5-java-json-libraries/)
* [PeopleSoft PeopleTools Tips &amp; Techniques</a> by Jim J. Marion](http://mhprofessional.com/product.php?isbn=0071664939)
* [JSON.simple in Jim's Blog](http://jjmpsj.blogspot.com/2010/04/json-encoding-in-peoplecode.html)
* [Tutorial: Using Ext JS, Servlets, JSON, MySQL and Tomcat on Fedora](http://java.sys-con.com/node/1201109)
* [Interesting blog on JSON numeric types from Public Object](http://blog.publicobject.com/2010/04/json-javascript-and-numeric-types.html)
* [Android as SOA player](http://blogs.eteration.com/blog/?p=978)

# Next Steps

* Auto marshalling and unmarshalling utils for Java Beans

# Links

* [JSON.org](http://json.org/)
* [Initial version of JSON.simple](http://json-simple.googlecode.com/files/json_simple.zip)

# About me

[Yidong Fang](http://www.linkedin.com/pub/yidong-fang/12/4b7/b2a)

# Acknowledgment

![YourKit](http://www.yourkit.com/images/yklogo.png)

YourKit is kindly supporting this open source project with its full-featured Java Profiler.
YourKit, LLC is the creator of innovative and intelligent tools for profiling Java and .NET applications. Take a look at YourKit's leading software products:

* [YourKit Java Profiler](http://www.yourkit.com/java/profiler/index.jsp)
* [YourKit .NET Profiler](http://www.yourkit.com/.net/profiler/index.jsp)
