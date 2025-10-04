# Choosing a Service Oriented Architecture for our system

## Context and Problem Statement

We are building a complaint management system which will be used by multiple different banks and a few different industries. We need to decide what the best architecture would be to use for a system like this. We would also need to consider the our projected users for this system, which should be a substantial amount as if we look at Barclarlys alone, they house 20 million customers within the UK.

## Considered Options

* Service Oriented Architecture
* Client Server Architecture
* Three Tier Architecture

## Decision Outcome

Chosen option: "Service Oriented Architecture"", because it is the only option that ticks the boxes on, scalability, multi-tenancy, extensibility and availability all at one. This would be more complex though compared to something like a three-tier design, but would provide the flexibility needed to incorporate future features, such as a chat bot and would help in supporting the growing user count and overall large user load that will be put on the system. Overall, it comes out best when thinking about scalability, extensibility and ticking the boxes of the stakeholders.

### Consequences

* Good, because the system will be really scalable, and should be able to handle large amounts of users, helping with the projected yearly userbase growth of the system.

* Good, because the architecture will allow the system to be extensible, making it really easy in the future to add extra features such as a chat bot.

* Good, because it will make managing multi tenancy a lot simpler, as all the components and services will operate seperate of eachother, making it a lot easier to isolate certain features and views.

* Bad, because it will be a lot more complex to integrate in this architecure, when comparing it to other styles such as three tier.

* Bad, because it will be hard to keep data consistant, as sharing data around the different components will be hard to manage.
