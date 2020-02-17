# EMBL : Create REST API which stores, update, retrieves and deletes Person 
[![build status](https://gitlab.cern.ch/c2mon/c2mon/badges/master/build.svg)](https://gitlab.cern.ch/c2mon/c2mon/commits/master)

The CERN Control and Monitoring Platform (C2MON) is a heterogeneous data acquisition and monitoring framework. It contains many useful features
such as historical metric persistence and browsing, command execution and alerting. It can be suitable for building many different types
of monitoring and control system or a full SCADA application.

## Documentation
See the current [reference docs][].

## Issue tracking
All C2MON issues are tracked and maintained within the [CERN JIRA][] system. Alternatively, you can send an email to c2mon-support@cern.ch.

## Release notes
Please have a look into the [CHANGELOG.md][] file.

## Milestone planning
[Find here][] the complete list of all existing version milestones.

## Downloading latest stable server tarball 

The C2MON server tarball can be downloaded from [CERN Nexus Repository](https://nexus.web.cern.ch/nexus/#nexus-search;gav~cern.c2mon.server~c2mon-server)

Please check also the [CHANGELOG.md] to find out the latest stable release version.

## Building from Source
C2MON uses a [Maven][]-based build system. In the instructions
below, `./mvnw` is invoked from the root of the source tree and serves as
a cross-platform, self-contained bootstrap mechanism for the build.

### Prerequisites

[Git][] and [JDK 8 update 152 or later][JDK8 build]

Be sure that your `JAVA_HOME` environment variable points to the `jdk1.8.0` folder
extracted from the JDK download.

#### IDEs

To reduce the boiler plate code we make use of [Lombok](https://projectlombok.org/), which requires to be [setup in your IDE](https://projectlombok.org/setup/overview) in order to compile the project.

### Check out sources
`git clone git@github.com:c2mon/c2mon.git`

### Compile and test; build all jars, distribution tarball, and docs
`./mvnw package -pl \!docs -DskipDocker=true`

## Contributing
[Pull requests][] are welcome; see the [contributor guidelines][] for details.

## License
C2MON is released under the [GNU LGPLv3 License][].

[Javadoc]: https://c2mon.web.cern.ch/c2mon/javadoc/
[reference docs]: http://c2mon.web.cern.ch/c2mon/docs/
[CERN JIRA]: https://its.cern.ch/jira/projects/CM
[GitHub issues]: https://github.com/c2mon/c2mon/issues
[CHANGELOG.md]: /CHANGELOG.md
[Find here]: https://gitlab.cern.ch/c2mon/c2mon/milestones?state=all
[Maven]: http://maven.apache.org
[Git]: http://help.github.com/set-up-git-redirect
[JDK8 build]: http://www.oracle.com/technetwork/java/javase/downloads
[Pull requests]: http://help.github.com/send-pull-requests
[contributor guidelines]: /CONTRIBUTING.md
[GNU LGPLv3 License]: /LICENSE