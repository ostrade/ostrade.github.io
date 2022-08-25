# Technologies

## gRPC and Protobuf Defined Interfaces
The interfaces will be defined using [Google Protobuf](https://developers.google.com/protocol-buffers) which is a language-neutral, platform-neutral, extensible mechanism for serializing structured data. You define how you want your data to be structured once, then you can use special generated source code to easily write and read your structured data to and from a variety of data streams and using a variety of languages.

## Integrations
Internal integrations will be managed using [Kafka](https://kafka.apache.org), an open-source distributed event streaming platform used by thousands of companies for high-performance data pipelines, streaming analytics, data integration, and mission-critical applications.

## Service Implementations
Implementations will use [Quarkus](https://quarkus.io), a Kubernetes Native Java stack tailored for OpenJDK HotSpot and GraalVM, crafted from the best of breed Java libraries and standards.

## Persistence
There will be two layers of persistence available. 

* [Infinispan](https://infinispan.org) - an open-source in-memory data grid that offers flexible deployment options and robust capabilities for storing, managing, and processing data. Infinispan provides a key/value data store that can hold all types of data, from Java objects to plain text. Infinispan distributes your data across elastically scalable clusters to guarantee high availability and fault tolerance, whether you use Infinispan as a volatile cache or a persistent data store.
* [PostgreSQL](https://www.postgresql.org) - an open source object-relational database system with over 30 years of active development that has earned it a strong reputation for reliability, feature robustness, and performance.

## Deployment and CICD
The primary deployment target is [OpenShift](https://www.redhat.com/en/technologies/cloud-computing/openshift), an enterprise-ready Kubernetes container platform built for an open hybrid cloud strategy. It provides a consistent application platform to manage hybrid cloud, multicloud, and edge deployments. We will use [Red Hat OpenShift Pipelines](https://www.redhat.com/en/topics/devops/what-cicd-pipeline#red-hat-openshift-pipelines) for CICD. It is a Kubernetes-native CI/CD solution which builds on Tekton to provide a CI/CD experience through tight integration with OpenShift and Red Hat developer tools. OpenShift Pipelines is designed to run each step of the CI/CD pipeline in its own container, allowing each step to scale independently to meet the demands of the pipeline.
