# ADR 5: Cloud Provider
We need to choose a cloud provider to host our application. The cloud provider that we choose should allow us to build and deploy our application quickly and begin producing value quickly. The cloud provider must satisfy the following criteria:

* Be able to provide infrastructure capable of supporting our LLM heavy workloads
* Provide a Kubernetes implementation
* Allow us to quickly scale up or down 

## Decision 
We will use AWS as our Cloud Provider

## Rationale 
Most cloud providers satisfy our needs. Our team is most familiar with AWS, which heavily influenced our choice. 

We foresee a future where we might need to build and maintain a private cloud, but in the short term AWS allows us to quickly build our product and get it into our customer's hands.

## Status
Proposed

## Consequences
* We will use EKS for our Kubernetes platform
* As we grow costs in AWS may become prohibitive 
