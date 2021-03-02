
## What is Moquette?

[![Build Status](https://api.travis-ci.org/moquette-io/moquette.svg?branch=master)](https://travis-ci.org/moquette-io/moquette)

* [Documentation reference guide](http://moquette-io.github.io/moquette/) Guide on how to use and configure Moquette
* [Google Group](https://groups.google.com/forum/#!forum/moquette-mqtt) Google Group to participate in development discussions.

Moquette aims to be a MQTT compliant broker. The broker supports QoS 0, QoS 1 and QoS 2.

Its designed to be evented, uses Netty for the protocol encoding and decoding part.
 
## Embeddable

[Freedomotic](https://www.freedomotic-iot.com/) is an home automation framework and uses Moquette embedded to interface with MQTT by a specific [plugin](https://freedomotic-user-manual.readthedocs.io/en/latest/plugins/mqtt-broker.html). 

Moquette is also used into [Atomize Spin](http://atomizesoftware.com/spin) a software solution for the logistic field.

Part of moquette are used into the [Vertx MQTT module](https://github.com/giovibal/vertx-mqtt-broker-mod), into [MQTT spy](http://kamilfb.github.io/mqtt-spy/)
and into [WSO2 Messge broker](http://techexplosives-pamod.blogspot.it/2014/05/mqtt-transport-architecture-wso2-mb-3x.html).

## Try the demo instance

Point your browser to [cloud instance](http://broker.moquette.io), request an account then use it from your MQTT clients.

## 1 minute set up

Start play with it, download the self distribution tar from [BinTray](https://bintray.com/artifact/download/andsel/generic/moquette-0.12.1.tar.gz) ,
the un untar and start the broker listening on `1883` port and enjoy!

```
tar xvf moquette-distribution-0.12.1.tar.gz
cd bin
./moquette.sh
```

Or if you are on Windows shell

```
 cd bin
 .\moquette.bat
```

## Embedding in other projects

To embed Moquette in another maven project is sufficient to include a repository and declare the dependency: 

```
 
   
     bintray 
     https://jcenter.bintray.com 
     
       true 
     
     
       false 
     
   
 
```

Include dependency in your project: 

```
 
       io.moquette 
       moquette-broker 
       0.12.1 
 
```

## Build from sources


After a git clone of the repository, cd into the cloned sources and: `./gradlew clean moquette-distribution:distMoquetteTar` or
`./gradlew clean moquette-distribution:distMoquetteZip`.


In distribution/build directory will be produced the selfcontained file for the broker with all dependencies and a running script. 
  

---

If you like Moquette you can support us by donating.

 
   
 


 # 良心友情链接

[腾讯QQ群快速检索](http://u.720life.cn/s/8cf73f7c)

[软件免费开发论坛](http://u.720life.cn/s/bbb01dc0)