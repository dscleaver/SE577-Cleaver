# ADR 3: Service Implementation Language
We need to choose an implementation language for our server side work. Javascript, Kotlin, and Swift are almost required languages for our front-end work, but we want to be consistent with our language on the server side. The language that we choose must meet the following criteria:

* Mainstream enough to have a decent hiring pool of development talent
* Allow our development team to contribute to SuperAGI
* Provide a web service framework

## Decision 
We will use Python as our implementation language for services.

## Rationale 
SuperAGI is implemented in Python which limited our options in regards to choosing a language consistent with SuperAGI. Fortunately, Python is a mainstream development language with several options for web service frameworks.

We considered Go, but it would have required hiring of polyglot programmers that could support both Go and Python.

## Status
Proposed

## Consequences
* Python is an interpreted language which may introduce performance issues
* We can also hire from the SuperAGI contributors to support the SuperAGI project and our own goals 

