# ![Numenta Logo](http://numenta.org/images/numenta-icon128.png)  
# htm.java

<br>

[![htm.java awesomeness](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](http://cogmission.ai) [![AGI Probability](https://img.shields.io/badge/AGI%20Probability-97%25-blue.svg)](http://numenta.com/#hero) [![Coolness Factor](https://img.shields.io/badge/Coolness%20Factor-100%25-blue.svg)](https://github.com/numenta/htm.java-examples) [![Build Status](https://travis-ci.org/numenta/htm.java.png?branch=master)](https://travis-ci.org/numenta/htm.java) [![Coverage Status](https://coveralls.io/repos/numenta/htm.java/badge.svg?branch=master&service=github)](https://coveralls.io/github/numenta/htm.java?branch=master) [![Maven Central](https://maven-badges.herokuapp.com/maven-central/org.numenta/htm.java/badge.svg)](https://maven-badges.herokuapp.com/maven-central/org.numenta/htm.java) [![][license img]][license] [![docs-badge][]][docs] [![Gitter](https://badges.gitter.im/Join  
Chat.svg)](https://gitter.im/numenta/htm.java?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)

<br>

#### [Official](https://github.com/numenta/htm.java/issues/193)  **Java&trade;** version of...
## Hierarchical Temporal Memory [(HTM)](http://numenta.com/learn/principles-of-hierarchical-temporal-memory.html)

**Community-supported & ported from the** [Numenta Platform for Intelligent Computing (NuPIC) ](https://github.com/numenta/nupic) python project.

_**NOTE: Minimum JavaSE version is 1.8**_

<br>

***

#### Demos & Examples: [HTM.java-examples](https://github.com/numenta/htm.java-examples) repository

***

<br>

### Recent News Items...
* [HTM.java] Recieves [Docker Reference-Build Implementation](https://github.com/numenta/htm.java/wiki/Build-Instructions#reference-build-environment) (03/26/2016)  
* **HTM.java Becomes Build-able With OpenJDK** (03/26/2016)  
* [HTM.java Receives Speed Increase Optimizations & Roots out Indeterminacy!](http://lists.numenta.org/pipermail/nupic-hackers_lists.numenta.org/2016-January/004422.html) (01/05/2016)
* **Network API Rework** for [improved input classification!](http://www.cogmission.ai/2015/10/23/putting-out-fires-with-gasoline/) - (10/23/2015)
* **Use HTM.java for the new** [Numenta HTM Challenge!](http://htmchallenge.devpost.com) - (Sept. 18th - Nov.6th)
* **HTM.java Receives newly updated and re-written TemporalMemory and MonitorMixinFramework** - for test reporting and monitoring (08/23/2015)

### [News Archives...](https://github.com/numenta/htm.java/wiki/News-Archives...)
* See a glimpse of htm.java's history and read about significant events in its development.  


### View the [Change Log](https://github.com/numenta/htm.java/blob/master/CHANGELOG.md) (Updated! 2016-03-27)
* Change log itemizes the release history.
* Contains an **"Unreleased" section** which lists changes coming in the next release as they're being worked on - (should help users keep in touch with the current evolution of htm.java)

***

For a more detailed discussion of <b>htm.java</b> see: <BR>
* [htm.java Wiki](https://github.com/numenta/htm.java/wiki)
* [Java Docs](http://numenta.org/docs/htm.java/)

See the [Test Coverage Reports](https://coveralls.io/jobs/4164658) - For more information on where you can contribute! Extend the tests and get your name in bright lights!

For answers to more detailed questions, email the [nupic-discuss](http://lists.numenta.org/mailman/listinfo/nupic_lists.numenta.org) mailing list, or chat with us on Gitter.

[![Gitter](https://img.shields.io/badge/gitter-join_chat-blue.svg?style=flat)](https://gitter.im/numenta/public?utm_source=badge)


For more detailed discussions regarding HTM.java specifically, come chat with us here: 

[![Gitter](https://img.shields.io/badge/gitter-join_chat-green.svg?style=flat)](https://gitter.im/numenta/htm.java?utm_source=badge)

See the blog: [Join the Cogmission](http://www.cogmission.ai)

***
<a name="callToArms"></a>
### Call to Arms: [HTM.java needs you!](https://github.com/numenta/htm.java/wiki/Call-To-Arms)

## Project Goals

The primary goal of this library development is to provide a Java version of NuPIC that has a 1-to-1 correspondence to all systems, functionality and tests provided by Numenta's open source implementation; while observing the tenets, standards and conventions of Java language best practices and development.

By working closely with Numenta and receiving their enthusiastic support and guidance, it is intended that this library be maintained as a viable Java language alternative to Numenta's C++ and Python offerings. However it must be understood that "official" support is (for the time being) currently limited to community resources such as the maintainers of this library and Numenta Forums / Message Lists and IRC:

 * [NuPIC Community](http://numenta.org/index.html#community)

***
## How Do I Get The Code? 

* **(A)** Instructions for developers who would like to contribute code back to our community.  (Fork)  
* **(B)** Instructions for those who would like to "fiddle around" with the code in thier own github repo.  (Clone)  
* **(C)** How to download Zipped or Tar'd Tagged Releases  (Download Zip or Tar)  

**A.** Developers who wish to make contributions are required to [Fork the htm.java repo](https://help.github.com/articles/fork-a-repo/) and then clone from their personal "Fork" of htm.java...
```
your_git_directory% git clone https://github.com/<your_github_username>/htm.java.git
```

**B.** Anybody who just wants to "play" with the code...
```
your_git_directory% git clone https://github.com/numenta/htm.java.git
```

**C.** [Proceed here](https://github.com/numenta/htm.java/releases) to download the latest tagged release (or older if you like)

_The instructions on the above link **(Fork the htm.java repo)** provide detail about how to fork github repos..._  

**In addition:** [a video is provided](https://www.youtube.com/watch?v=Yc3PKaT1knU) that explains Numenta's contributor rules and plenty of helpful tips on using git and other commands.

***
## Does My Code Work?

After download by clone or fork, execute a quick sanity check by running all the tests from within the /\<path to git repo\>/htm.java
```
gradle check  # Executes the tests and runs the benchmarks

--or--

gradle -Pskipbench check  # Executes the tests w/o running the benchmarks
```
**Note:** Info on installing **gradle** can be found on the wiki (look at #3.) [here](https://github.com/numenta/htm.java/wiki/Eclipse-Setup-Tips)

**Linux Gradle Issues?** [see the wiki here.](https://github.com/numenta/htm.java/wiki/Gradle---JAVA_HOME-Issue-Resolution)

**A [wiki](https://github.com/numenta/htm.java/wiki/Build-Instructions) with full build instructions for building HTM.java is available here:** [Build Instructions](https://github.com/numenta/htm.java/wiki/Build-Instructions) (This includes a no-java/gradle-guaranteed-build using the provided [Docker File](https://github.com/numenta/htm.java/blob/master/Dockerfile) as a reference build.) 

***
## For Developers: Usage & Project Integration  
**_(use this stuff within my own stuff)_**  

**NOTE:** The Java version of NuPIC **requires no installation** - just **USE** it!
* I Just Want A Simple Build!
* Using Build Managers

**Simple Build:** For convenience, the [libs](https://github.com/numenta/htm.java/tree/master/libs) directory contains all the dependency jars for those who just want to have a simple build.  

...  

**Build Managers:** Binary distributions may be included in your project using Gradle or Maven  
```
Gradle:  

dependencies {
    compile group: 'org.numenta', name: 'htm.java', version:'0.6.5'
}
```

```
Maven:  

<dependency>
    <groupId>org.numenta</groupId>
    <artifactId>htm.java</artifactId>
    <version>0.6.5</version>
</dependency>
```

``` 
Hot to get the latest SNAPSHOT build:

<dependency>
    <groupId>org.numenta</groupId>
    <artifactId>htm.java</artifactId>
    <version>0.6.6-SNAPSHOT</version>
</dependency>

You also may need to include a repositories entry:

<repository>
    <id>oss-sonatype</id>
    <name>oss-sonatype</name>
    <url>https://oss.sonatype.org/content/repositories/snapshots/</url>
    <snapshots>
        <enabled>true</enabled>
    </snapshots>
</repository>
```  

***
## Coding With htm.java

The easiest way to use the code is to use htm.java's **Network API**

Please refer to the [Network API Quick Start Guide](https://github.com/numenta/htm.java/wiki/NAPI-Quick-Start-Guide)
to get an idea of how to quickly and simply create your own network.

...and for more in-depth answers see:

[NAPI Overview](https://github.com/numenta/htm.java/wiki/NAPI-In-Depth-Component-Overview)

***
## Development Environment Installation

The following instructions are for setting up a development environment.

**NOTE:** For simple intructions see: [INSTALL.txt](https://github.com/numenta/htm.java/blob/master/INSTALL.txt) 

[Eclipse Environment Setup Wiki](https://github.com/numenta/htm.java/wiki/Eclipse-Setup-Tips)

An Eclipse IDE .project and .classpath file are provided so that the cloned project can be easily set up inside of Eclipse. For the time being, the Eclipse IDE is the only "pre-made" project configuration.

In addition, there are "launch configurations" for all of the tests and any runnable entities off of the "htm.java" main directory. These may be run directly in Eclipse by right-clicking them and choosing "run".

***
## The "Fancy Stuff" - Clustering and Parallelization

Some NuPIC Community members have created interesting projects which use htm.java's Network API to run Engine-Type clusters of multiple networks using streaming distributed libraries like [Akka](http://akka.io) and [Flink](https://flink.apache.org). See them here:

* [htm-moclu](https://github.com/antidata/htm-moclu) (Akka)
* [flink-htm](https://github.com/nupic-community/flink-htm) (Flink - some say it's a better [Spark](http://spark.apache.org))  

***
## To Follow Our Updates On Twitter

* [#HtmJavaDevUpdates](https://twitter.com/hashtag/HtmJavaDevUpdates?src=hash)


[license]:LICENSE.txt
[license img]:https://img.shields.io/badge/License-GNU%20Affero-blue.svg

[docs-badge]:https://img.shields.io/badge/API-docs-blue.svg?style=flat-square
[docs]:http://numenta.org/docs/htm.java/
