# Deciding against a Three Tier Architecture for our system

## Context and Problem Statement

We are building a complaint management system (CMS) which will be used by multiple different banks and potentially other industries. The system will need to handle millions of users (e.g. Barclays investor update states 20 million customers in the UK) but still keeping the system scalable, having proper multi tenancy and being extensible. A decision will need to be made on what architecture style would be suitable for this system.

## Considered Options

* Service Oriented Architecture
* Client Server Architecture
* Three Tier Architecture

## Decision Outcome

Chosen option: Not to use "Three Tier Architecture", because even though it is super simple and easy to understand, it would not scale very well and would be be more difficult than SOA to add features on in the future. Under a large load of users it would be difficult for the system to operate as three tier can be quite rigid and wouldn't scale well as everything would be tied to a single application server. This also means that as everything is bundled together it would be a lot more difficult than SOA to implement new feature as it would require a lot more tinkering and setting up. So, although it would be a lot simpler and quicker to implement, it would not provide the long term flexibility and scalability needed for this system.

### Consequences

* Good, because a three tier system is simple to undersyand and implement, which would allow for a quick turnaround on getting the system to production.

* Bad, because three tier would not be as scalable as needed for a projected userbase of this size. Dealing with millions of different users, accross different companies and industries would be too much for this architecture to handle in the long run.

* Bad, because it is not as extensible as is needed for a project like this. While you can still add features into a three tier style, it would require a lot more work than it would in an archicture like SOA.
