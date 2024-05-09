# ADR 4: Deployment Platform
We need a platform on which to deploy our application servers. The platform should allow us to:

* Scale components up and down
* Manage running instances
* Dynamically add independent isolated AI Agents

## Decision 
We will use Kubernetes as our deployment platform.

## Rationale 
Kubernetes has won the battle for container orchestration system. With Kubernetes as our target for deployment we will be more easily able to stand up our system in any cloud provider that we choose.

## Status
Proposed

## Consequences
* Cloud independent deployment platform
* We will need to build our system components into containers
* Deployment scripts for our selected cloud provider will need to be built

