---
layout: page
title: RuleScript
description: An extensible and verifiable language for query rewrite rules.
importance: 1
category: research
related_publications: true
---

RuleScript is a domain-specific language for expressing and verifying query optimization rules. The same rule descriptions can be used to generate implementations for different database systems.

I built code generators and implemented 34 rules for Apache Calcite and CockroachDB, demonstrating that the design can connect declarative rule specifications with practical database optimizers.

This work was conducted at the University of California, Berkeley with Prof. Alvin Cheung.

See the related [publication]({{ '/publications/' | relative_url }}) for the research details.
