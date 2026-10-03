---
layout: post
title: "Software Craftsmanship Is Dead. Long Live Software Craftsmanship."
subtitle: "A manifesto for engineers who refuse to be meat-proxies in the world."
description: "AI agents made messy code cheap to fix, so clean architecture lost its business case. The real problem now is knowledge debt, and craftsmanship returns when engineers demand it."
image: /assets/cover-software-craftsmanship.jpeg
date: 2026-10-03
---

<img class="post-cover" src="{{ site.baseurl }}/assets/cover-software-craftsmanship.jpeg" alt="Software Craftsmanship Is Dead. Long Live Software Craftsmanship.">

We lied to ourselves for twenty years.

We bought the books, argued about folder structures on Twitter, and wrote posts about domain-driven design. We convinced ourselves we were artisans, like furniture makers carefully joining hidden wood inside a cabinet. In reality, users do not care about your architecture.

Teammates rarely read refactoring pull requests, and the company does not track your test coverage. Clean code was mostly a psychological coping mechanism so we would not feel like factory workers stitching together third-party APIs.

The market tracks two things: whether the software works, and whether it makes or loses money.

Consider how organizations handle redundant systems. A team builds a clean, modern service with 3P observability and a full test pyramid, running alongside an older service doing roughly the same job but a mess of undocumented background scripts and scheduled tasks. When management decides to consolidate, they turn off the clean service.

It was modular enough to be safely unplugged. The legacy service survived because it held the business hostage. Nobody knew what those background jobs were doing, who depended on them, or what would break if they stopped. The mess won because replacing it carried too much risk. In enterprise software, technical debt is often structural job security.

> In enterprise software, technical debt is often structural job security.

For a long time, engineers argued that messy code eventually cost too much time and money to maintain. AI agents erased that constraint.

When a service crashes at night, an agent can loop through patches until the tests pass. When code gets coupled, context windows and cheaper inference models can parse the execution paths anyway. If an agent can untangle messy code in seconds for pennies, the financial case for clean architecture collapses. A messy service that used to cost developer hours now costs a small prompting budget.

This shift changes how people build software. People with no software background are building web and mobile apps with prompts, delivering work that used to require at least junior engineers.

Upper management notices this and starts treating developers as proxies for AI models. The expected job becomes pasting prompts, approving agent permissions, and running deploys.

While technical debt becomes cheaper to mask with compute, companies build up knowledge debt instead.

Knowledge debt happens when critical software handles core business operations while no one on the team understands how or why it works. When those background processes fail or an edge case breaks several AI-generated microservices at once, you cannot prompt your way out if no human understands the underlying system.

> Technical debt costs money. Knowledge debt costs understanding, and you cannot prompt it back.

<div class="section-divider"><span>◆</span></div>

Craftsmanship will not return because management asks for it. It returns when engineers demand it in their daily work.

Taking a stand against knowledge debt does not require rejecting AI tools or writing complex abstractions for fun. It means using code quality principles to keep cognitive load low enough that humans can maintain mental models of the software. Clean architecture is useful because it keeps systems comprehensible. Forcing AI agents to produce clean boundaries, explicit schemas, and modular designs ensures that engineers can still trace and debug execution paths when things break.

We maintain code quality so we can continue to understand what we build.

Software markets move in cycles. The current surge in rapid AI code generation and instant service creation will eventually run into a maintenance phase. As black-box architectures fail at scale and silent data issues go unnoticed, cheap code generation will show its hidden operational cost.

Engineers can push for lower knowledge debt in their own codebase while expecting better reliability and SLA standards from vendor software. The era of writing clean code as a personal hobby is over, but designing readable, maintainable systems remains practical engineering work that the market will eventually require.
