# Trends and Developments

A longitudinal analysis of how topics, tools, and ideas evolved across the Chiang Mai AI community meetups. Last updated after the March 28, 2026 session.

## From tools to agents to systems to organizations

In June-August 2025, people discussed individual tools (PG Vector, Supabase, git worktree). By October, it shifted to agent workflows ("Samantha" buying domains overnight, the Surgeon vs Tool-Caller split). By early 2026, it's multi-agent orchestration (sub-agents, swarms, control planes). And by March 2026, someone is presenting an enterprise rollout to a 30-person team with compliance requirements. The abstraction level kept rising.

## The Claude Code arc

Claude Code started as the dominant tool everyone used for everything. Then Codex appeared and people discovered it was better at coding. By early 2026, nearly everyone in the room runs a split workflow: Codex for coding, Claude for planning/reviewing/personal agents. By March 2026, the presenter said "I don't use Claude for coding at all anymore" and nobody disagreed.

## Token economics from paradise to panic

Early sessions barely mentioned cost. Then rate limits appeared and people complained. The $200 plan became mandatory for power users. By March 2026, an OpenAI exec said unlimited plans are unsustainable, and one week later Anthropic started reducing allocations. The group's own prediction came true in 7 days. The Uber/Lyft analogy ("we're in the burning VC cash phase") became a recurring theme.

## Security went from afterthought to first-class concern

In June-October 2025, security was barely mentioned. Then Simon Willison's quote appeared ("anybody who can get their tokens into your context should be considered to have full control"). By November, there were dedicated discussions on prompt injection, data exfiltration via plugins, and a DEFCON talk recommendation. By March 2026, there are full presentations on agent security architecture with gradual trust models.

## The context window paradox

This thread runs through almost every session. The 200k window caused "context anxiety" (the model rushing as it filled up). The 1M window was supposed to fix it but most people are still too scared to go past 300k. Sub-agents emerged as a workaround (fresh context per task), then skills as lazy-loading (150k to 2k tokens). But the fundamental tension of "more compute = better results = more tokens = more cost" never resolved.

## Structural drift as the central unsolved problem

First mentioned around November 2025, it became the central unsolved problem by March 2026. Agents writing to file systems create inconsistent schemas over time. After a thousand files, searches break. Open Claw users report burning millions of tokens on simple searches after two months. Multiple solutions were proposed (the ALS compiler, LLM hooks as validators, fine-tuned local models for search), but no consensus emerged. The term "token burn" was proposed as the new equivalent of "technical debt."

## Agent-to-agent communication

Raised repeatedly from October 2025 onward. Google's A2A protocol, OpenAI's commerce protocol, MCP servers, remote tool use. Every session someone brings it up, and every time the conclusion is "we need a standard but don't have one yet." By March 2026, the practical approach most people settled on was "just go with whichever protocol gets the largest user base."

## The developer role shift

A consistent theme from August 2025 onward. Developers are transitioning from hands-on coders to managers of agents, architects, and orchestrators. The value is no longer in writing every line of code but in breaking down complex problems, defining architecture, and setting guardrails. Jensen Huang's statement that engineers should be burning $250k in tokens reinforced this. The group noted that token usage correlates inversely with task novelty: classical software should consume massive tokens, bleeding-edge work cannot.

## Open source vs closed source tension

A consistent undercurrent across all sessions. Local models are always tested and always found lacking for frontier tasks. But the desire for self-hosting never went away. China's Open Claw explosion (100k+ instances) showed massive demand for accessible AI. The group remained pragmatic: use closed source for production, keep an eye on open source for cost optimization and edge computing.

## Community evolution

The group went from 3-6 people at a single Saturday session at Morestto to three weekly series (Saturday, Wednesday, Friday) with lightning talks, guest presentations, and panels at The Kannas. The format evolved from "let's look at the news" to structured presentations followed by discussion. A Bangkok sister community spawned. An Anthropic-sponsored event was hosted at CMU in December 2025.

## The emotional arc

October 2025 had a candid discussion about burnout and 12-15 hour coding sprints. "Tooling anxiety" was coined the same month. By early 2026, people developed coping strategies: the "underwater" method (ignore all new tools until your project ships), project-based focus, and community sourcing ("rely on the meetup to filter the 1% of news that actually matters"). By March 2026, the tone is more pragmatic. Less FOMO, more "burn the VC money while you can" and focus on what actually works.

## The pace never slowed

Every single session, without exception, someone mentions a new tool, model, or framework that didn't exist the previous week. If anything, it accelerated.
