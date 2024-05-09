# ADR 2: Core LLM 
Our choice of SuperAGI allows our AI agents to be flexible in their choice of underlying Large Language Model (LLM). When choosing a Large Language Model, we must consider the following factors:

* The cost of running the model
* Privacy guarantees
* Our ability to fine tune the model for each agent

## Decision 
We will use Meta's Llama 3 for our LLM model.

## Rationale 
Llama 3 allows us to run our own private instances of the model. Additionally there are many fine-tuned versions of Llama 3 and we can create our own fine-tuned versions to support the specific needs of our AI Agents. 

OpenAI's GPT-4 was another possible model choice, which we rejected. While we could guarantee that OpenAI would not keep or use data that we send to their model, we can not fine tune GPT-4 to our specific needs.

## Status
Proposed

## Consequences
* We will need to stnad up infrastructure that can run Llama 3
* Llama 3 gives us the flexibility that we require to create specific task specific AI Agents
