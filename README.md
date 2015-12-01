# HttpClientAndroidLib
A mirror of https://code.google.com/p/httpclientandroidlib by [Dirk Boye](https://github.com/dirkboye/); 
a Android port of Apache's HttpComponents library (version 4.2.3).

The purpose of this project is to resolve issues in which Java projects that depend on Apache's HttpComponents 
version 4.2.x do not work properly on Android. This library provides a solution to this (though it usually requires forking the
library you want to use and changing the code).

The reason for the mirror is to provide a Maven repo through jitpack.io.


##Usage
To get HttpClientAndroidLib as a dependency in you Maven project, first add the jitpack.io repo:
``` xml
<repository>
  <id>jitpack.io</id>
  <url>https://jitpack.io</url>
</repository>
```
Then add it to your dependencies:
``` xml
<dependency>
  <groupId>com.github.emptyflash</groupId>
  <artifactId>httpclientandroidlib</artifactId>
  <version>1.1.3</version>
  <classifier>ant-jar</classifier>
</dependency>
```

Then in your code, replace all occurences of `org.apache.http` with `ch.boye.httpclientandroidlib`
