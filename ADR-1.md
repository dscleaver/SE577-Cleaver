# ADR 1: AI Agent Framework
[AI Agents](https://aws.amazon.com/what-is/ai-agents/) are a necessary part of BizBuddy. The rise of LLMs has brought new renewed interest in autonomous agents that can plan and act on their own. [Many open source projects](https://www.taskade.com/blog/top-autonomous-agents/) have been created that can be used to build our autonomous agents. We need to choose one of these agent frameworks. The framework that we choose should allow us to

* plug in any underlying LLM model that we want
* plug in any vector database that we require
* add new information sources to the AI Agent
* add new actions for the AI Agent to take

## Decision 
We will use SuperAGI to build our AI Agents.

## Rationale 
SuperAGI allows us to pick and choose from a wide variety of already implemented
integrations, and we can easily extend the project to build the ones that our AI
Agents will need.

## Status
Proposed

## Consequences
* We can trial multiple LLM and vector database implementations to find the ones
  that work best for our agents
* Our programmers will need to be comfortable with Python to extend SuperAGI's base
  functionality
