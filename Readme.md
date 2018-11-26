# CKAD
CNCF Certified Kubernetes Application Developer (CKAD)



Online resources that will help you prepare for taking the Certified Kubernetes Application Developer (CKAD) Certification exam.

**Disclaimer:** *This is not likely a comprehensive list as the exam will be a moving target with the fast pace of k8s development - please make a pull request if there something wrong or that should be added, or updated in here.*

* [CNCF Exam Curriculm repository](https://github.com/cncf/curriculum)
* [CKAD Candidate Handbook](https://www.cncf.io/certification/candidate-handbook)
* [CKAD Exam Tips](https://www2.thelinuxfoundation.org/ckad-tips)
* [FAQs](https://www.cncf.io/certification/expert/cka/faq/)


## Before you begin

You need to have a Kubernetes cluster, and the kubectl command-line tool must be configured to communicate with your cluster. If you do not already have a cluster, you can create one by using [Minikube](https://kubernetes.io/docs/getting-started-guides/minikube), or **you can use one of these Kubernetes playgrounds:**

* [Katacoda](https://www.katacoda.com/courses/kubernetes/playground)
* [Play with Kubernetes](http://labs.play-with-k8s.com/)

***Note: Both katacoda and PWK are free, you just need Google/GitHub/Docker account login to access.***

##Few additional Resources
* [K8s from Scratch](https://kubernetes.io/docs/setup/scratch/)
* [K8s Up & Running book by Hightower](http://shop.oreilly.com/product/0636920043874.do)
* [K8s the Hard way tutorial by Hightower](https://github.com/kelseyhightower/kubernetes-the-hard-way)

**Practice, Practice and Practice** 

# CKAD Curriculum V1.0

## Core Concepts - 13%
* [Understand kubernetes API Primitives](https://kubernetes.io/docs/concepts/overview/kubernetes-api/)
* Create and configure basic Pods
  * [Pod Overview](https://kubernetes.io/docs/concepts/workloads/pods/pod-overview/)
  * [Pod lifecycle](https://kubernetes.io/docs/concepts/workloads/pods/pod-lifecycle/)
  * [configure Pods and containers](https://kubernetes.io/docs/tasks/configure-pod-container/)

## Multi-Container Pods - 10%
* [Understand Multi-Container Pod design patterns (e.g: ambassador, adapter, sidecare)](https://kubernetes.io/blog/2015/06/the-distributed-system-toolkit-patterns/)

## Pod Design - 20%
* Understand how to use Labels, Selectors, and Annotations.
  * [Labels & Selectors](https://kubernetes.io/docs/concepts/overview/working-with-objects/labels/)
    * [Using labels effectively](https://kubernetes.io/docs/concepts/cluster-administration/manage-deployment/#using-labels-effectively)
  * [NodeSelector](https://kubernetes.io/docs/concepts/configuration/assign-pod-node/)
  * [Annotations overview](https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations/)
    * [kubectl annotate](https://kubernetes.io/docs/reference/generated/kubectl/kubectl-commands#annotate)
* Understand Deployments and how to perform rolling updates.
  * [deployments](https://kubernetes.io/docs/concepts/workloads/controllers/deployment/)
  * [rolling updates](https://kubernetes.io/docs/tutorials/kubernetes-basics/update-intro/)
* [Understand Deployments and how to perform rollbacks.](https://kubernetes.io/docs/concepts/workloads/controllers/deployment/#rolling-back-a-deployment)
* Understand Jobs and CronJobs.
  * CronJobs
    * [Overview](https://kubernetes.io/docs/concepts/workloads/controllers/cron-jobs/)
    * [Running automated tasks with CronJob](https://kubernetes.io/docs/tasks/job/automated-tasks-with-cron-jobs/)
  * Jobs
    * [Overview](https://kubernetes.io/docs/concepts/workloads/controllers/jobs-run-to-completion/)
    * [Parallel processing using Expansions](https://kubernetes.io/docs/tasks/job/parallel-processing-expansion/)
## Configuration - 18%
* [Understand ConfigMaps](https://kubernetes.io/docs/tasks/configure-pod-container/configure-pod-configmap/)
  * [Configure redis using ConfigMap](https://kubernetes.io/docs/tutorials/configuration/configure-redis-using-configmap/)
* [Understand SecurityContexts](https://kubernetes.io/docs/tasks/configure-pod-container/security-context/)
  * [SecurityContext v1 core](https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.10/#securitycontext-v1-core)
  * [Tuning Docker with the newest security enhancements](https://opensource.com/business/15/3/docker-security-tuning)
* [Define an application's resources requirements](https://kubernetes.io/docs/concepts/configuration/manage-compute-resources-container/)
* [Create & consume Secrets](https://kubernetes.io/docs/concepts/configuration/secret/)
* [Understand ServiceAccounts](https://kubernetes.io/docs/tasks/configure-pod-container/configure-service-account/)

## Observability - 18%
* Understand LivenessProbes and ReadinessProbes
  * [LivenessProbe](https://kubernetes.io/docs/tasks/configure-pod-container/configure-liveness-readiness-probes/)
  * [ReadinessProbe](https://kubernetes.io/docs/tasks/configure-pod-container/configure-liveness-readiness-probes/#define-readiness-probes)
* Understand container logging
  * [Logging](https://kubernetes.io/docs/concepts/cluster-administration/logging/)
  * [Using StackDrive](https://kubernetes.io/docs/tasks/debug-application-cluster/logging-stackdriver/)
* Understand how to monitor applications in Kubernetes
* Understand debugging in Kubernetes
  * [Application introspection](https://kubernetes.io/docs/tasks/debug-application-cluster/debug-application-introspection/)
  * [Services](https://kubernetes.io/docs/tasks/debug-application-cluster/debug-service/)

## Services & Networking - 13%
* [Understand Services](https://kubernetes.io/docs/concepts/services-networking/service/)
* [Demonstrate basic understanding of NetworkPolicies](https://kubernetes.io/docs/concepts/services-networking/network-policies/)
