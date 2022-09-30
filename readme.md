# IBM Digital Business Automation - Process Automation Manager Open Edition - Quick Start

This repository contains various tools, scripts, and product extensions useful for managing `IBM Process Automation Manager Open Edition` projects.

## Tool & Environment Requirements

The following tools are required to be installed on the developer workstation or on the machine performing CI/CD pipeline builds.  Please follow the link in order to download and install the various tools:

1. [**Maven**](https://maven.apache.org) - Required in order to perform Maven builds on the desktop.  
2. [**Git Client**](https://git-scm.com) - Required in order to clone and make changes to the project GIT repositories
3. [**JDK 11**](https://www.oracle.com/java/technologies/downloads/) - Requires Java 11 at this time
4. [**GraalVM (Optional)**](https://www.graalvm.org//) - Required if you want to test NATIVE compilation and deployment
5. [**VS Code IDE**](https://code.visualstudio.com/download) - An IDE is required, VS Code IDE is the default.  While you can use any IDE you wish, the embeddable editors are only available for VS Code.

*_Once you have installed VS Code, you can go to the Extensions Marketplace and install the `Kogito Bundle` for BPMN, DMN, and Test Scenarios_*.

## How To Build

This repository is built using `mvn clean install` by either the CI/CD pipeline or on a local developer workstation.  If deploying artifacts to an enterprise Maven repository, please use `mvn clean deploy`, which requires configuration of the `distributionManagement` section of your project's parent pom.xml.

## Repository Modules

This repository is organized in a series of modules:  

1.  [**Adaptors**](./adaptors/readme.md) - A set of legacy adaptors and product extensions used to augment the functionality of the legacy aspects of IBM Decision Manager Open Edition.  
2.  [**Maven**](./maven/readme.md) - A set of Maven extensions, such as custom archetypes and plugins, used to augment the functionality of IBM Decision Manager Open Edition.
3.  [**Scripts**](./scripts/readme.md) - A set of scripts useful for using various adaptors and maven extensions.
4.  [**Samples**](./samples/readme.md) - A set of sample applications generated using this kick-start repository.

## Additional Information (*Appendicies*)
This repository is focused on business automation using the **IBM Decison Manager Open Edition** product, which in turn relies on various open source tools and technology. The following online documentation is available in order to learn various aspects of these tools:

- [**Apache Maven**](https://maven.apache.org/) is a free and open source software project management and comprehension tool. Based on the concept of a project object model (POM), Maven can manage a project’s build, reporting and documentation from a central piece of  information. A **getting started guide** is available [here](http://maven.apache.org/guides/getting-started/).
- [**Git**](https://git-scm.com//) is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency. There is a **handbook** available [here](https://guides.github.com/introduction/git-handbook/), as well as various **guides** for learning and working with Git available [here](https://guides.github.com/
- [**Quarkus**](https://quarkus.io) Quarkus was created to enable Java developers to create applications for a modern, cloud-native world. Quarkus is a Kubernetes-native Java framework tailored for GraalVM and HotSpot, crafted from best-of-breed Java libraries and standards. The goal is to make Java the leading platform in Kubernetes and serverless environments while offering developers a framework to address a wider range of distributed application architectures.
- [**Kogito**](https://kogito.kie.org) Kogito is designed from ground up to run at scale on cloud infrastructure. If you think about business automation think about the cloud as this is where your business logic lives these days. By taking advantage of the latest technologies (Quarkus, knative, etc.), you get amazingly fast boot times and instant scaling on orchestration platforms like Kubernetes.
- [**IBM Business Automation Manager Open Edition**](https://www.ibm.com/docs/en/ibamoe?topic=getting-started-business-automation-manager-open-editions) IBM Business Automation Manager Open Editions, which consists of IBM Process Automation Manager and IBM Decision Manager Open Edition, offer developers the ability to build cloud-native applications that automate business operations. IBM Process Automation Manager Open Edition is a platform for developing containerized microservices and applications that automate processes and business decisions. IBM Decision Manager Open Edition, a subset of Process Automation Manager Open Edition, is a separately available platform for developing containerized microservices and applications that automate business decisions, including complex event processing.
