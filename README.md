# ![ValGraph.png](ValGraph.png) ValGraph

## Contents

- [!ValGraph.png ValGraph](#-valgraph)
  - [Contents](#contents)
  - [Summary](#summary)
  - [Thesis](#thesis)
  - [License](#license)

<a name="summary"></a>

## Summary

a delightful low-code GraphQL testing tool

<a name="thesis"></a>

## Thesis

**Legs**:

1. Low / no-code tooling is enabling more people to be involved in product without accreditation or engineering background.
   ex: `Figma`, `AirTable`, `Tableau` - business analysts can now be involved in product design, engineering, and analytics
2. Developers are increasingly being spread-thin as roles consolidate in the industry. 10 years ago, it wasn't uncommon to see a Software Engineer, QA Engineer, Database Admin, and UX Engineer working in harmony. Today, all of these roles have been compacted into the Full-Stack Engineer.
3. Microservices are exploding in popularity and more services are being [API-ified](https://www.notboring.co/p/apis-all-the-way-down). With this trend, technologies are emerging that make interfacing with disparate data streams easier. [GraphQL](https://graphql.org/) is the one I'm betting on.
   _(Sidenote: I understand this makes this tool low-TAM, but the [schema introspection](https://graphql.org/learn/introspection/) functionality will make the end product so much better)_
4. E2E + Integration testing is hard and it's often the most [useful](https://testingjavascript.com/). (3) makes this even more important.

**Dream the Dream**:

`ValGraph` is a low-code platform that makes writing automated GraphQL E2E tests easy and efficient. Moreover, since the tests are intended to be run against a GraphQL endpoint, the tool will allow customers to ping their service live and verify their SLA. A SaaS offering on top of the tool makes testing cheap in cost and in labor.

**Example**:

A PM is tasked with writing a spec for new functionality on the team's GraphQL endpoint. Rather than writing a word document, he writes some test cases and explanations using `ValGraph`.

A software engineer takes these test cases and builds a prototype running on her local machine. She checks in the code and adds some `ValGraph` test cases as well.

A dev-ops engineer takes both the checked in code and the test cases and deploys them to production. They sets up the `ValGraph` configuration to ping the live server every 2 minutes with all the test cases setup by PM and dev.

_3AM in the morning_: a micro-service the GraphQL endpoint uses faces a regression. Because `ValGraph` is pinging the endpoint every 2 minutes, a test cases fails and the on-call dev gets a notification on `PagerDuty` before any customers feel impact. She fails over to the previous build and an embarrassing crisis is averted.

<a name="license"></a>

## License

Shit if I know
