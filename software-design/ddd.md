# Domain-Driven Design

Domain-Driven Design is an approach of bringing software closer to the problem
domain.

DDD helps establish boundaries between domain problems and form autonomous
teams around this boundaries.

---

> DDD is about primarily about modelling a ubiquitous language in an explicitly
> bounded context.

Vaughn Vernon / Domain-Driven Design Distilled

---

Enigneers collaborate with domain experts to form a so-called ***ubiquitous
language***. This language is later used by both parties to talk about problems.
However, ubiquitous language is *context dependent* - 'Customer Rating' has
different meanings for Sales and Risk Management teams.

The limit of applicability of the ubiquitous language is called ***bounded
context***.

One thing to note is that one grand-unified model doesn't work well. It makes
more sense to come up with smaller models, in other word have multiple *bounded
context*.

Ideally, software model should reflect *ubiquitous language*.

Bounded contexts must be loosely coupled.

Well defined bounded contexts help increase autonomy between teams.

**Value objects** - immutable objects that help describe and measure thing (e.g.
Email, Money). They help with building domain-specific abstractions.

**Entity** - represent a "thing" in a system that have identity and a lifecycle.
It can consist of other entities and value objects. It is easier to think of an
entity as a unit of behaviour.

**Aggregates** - a consistency boundaries between aggreates. Entities are always
consistent in a specific aggreagate, but they are eventually consistent between
aggregates. Aggregate has ***root entity*** which host mutating commands of the
child entity. Often, aggregate is a mental concept (doesn't present in the
codebase). To establish boundaries between aggregates it is helpful to look for
conceptual wholes - which aggregate can be instantiated, queried or modified
independently of other aggregates. Also use a *delete rule of thumb* - is
keeping this aggregate make sense if I remove that aggregate.

**Factories** - encanpsulates the logic of creating *creation*
entities/aggregates.

**Repositories** - responsible for storing and retrieving aggregates.

**Domain event** - something interesting that affects the domain or something
that happens in the domain and is important to domain experts.

As for software architecture DDD it is good to separate your domain layer
from frameworks/data storage you are using.

## Links

[Robert Smallshire - Domain Driven Design Patterns in Python](https://www.youtube.com/watch?v=Ru2T4fu3bGQ)
[If You’re Building Microservices, You Need to Understand What a Bounded Context is](https://medium.datadriveninvestor.com/if-youre-building-microservices-you-need-to-understand-what-a-bounded-context-is-30cbe51d5085)
[Best Practice - An Introduction To Domain-Driven Design](https://docs.microsoft.com/en-us/archive/msdn-magazine/2009/february/best-practice-an-introduction-to-domain-driven-design)
[Domain Events vs. Event Sourcing](https://www.innoq.com/en/blog/domain-events-versus-event-sourcing/)
