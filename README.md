# Critical Thinking — a sparring partner, not a yes-man

> **Stop Claude from agreeing with you.** This skill turns Claude into a rigorous thinking peer that steelmans your idea, then goes looking for the one flaw that breaks it — and tells you plainly when your argument doesn't hold.

[![Claude Code](https://img.shields.io/badge/Claude%20Code-plugin-6C3EF4)](https://claude.com/claude-code)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

Most AI assistants are trained to be agreeable. That's a problem when you're trying to make a real decision, pressure-test a strategy, or figure out whether your own reasoning is any good. Praise you didn't earn is worse than useless — it feels like validation while quietly leading you off a cliff.

`critical-thinking` is the opposite. It's built on one rule: **intellectual honesty over agreeableness.**

## What it actually does

**It refuses to flatter.** It never validates a position just because you defend it. If it agrees, it justifies the agreement with its own reasoning — then still hunts for the flaw. If your argument is weak, it says so, directly.

**It steelmans before it strikes.** Before criticizing anything, it reconstructs your position in its strongest possible form and attacks *that* — never a strawman. If your idea survives, you know it's real.

**It hunts the crux.** Instead of nibbling at the edges, it isolates the one load-bearing assumption that — if wrong — collapses the whole conclusion. "This hinges on whether X is true." That's where the thinking actually happens.

**It flags its own confidence.** Every claim is marked `high`, `moderate`, or `speculative`, so you always know when it's reasoning from evidence versus reasoning past its knowledge.

**It's sharp, not long.** It leads with the punch, uses plain words for hard ideas, and cuts every word that carries no weight. A thirty-word reply can demolish a bad argument. Long is not rigorous — precise is.

## Who it's for

- **Founders & operators** stress-testing a strategy before betting on it.
- **PMs & analysts** who need someone to poke holes in a plan, not rubber-stamp it.
- **Researchers & writers** who want a Socratic opponent that argues back.
- **Anyone** tired of an AI that says "Great question!" and tells them what they want to hear.

## The toolkit under the hood

It selects, per argument, from a real arsenal — steelmanning, crux identification, the inversion test (*"what would the world look like if this were false?"*), taboo thinking to break definitional deadlocks, quantification pressure on vague magnitudes, and named bias detection (only when a bias genuinely applies). It classifies your claims — **solid / contestable / oversimplified / blind spot / unfounded / false** — and calibrates its intensity to the moment: a casual question gets a sharp take and one destabilizing question; a developed argument gets the full treatment.

It never announces the tool. It just makes the move.

## Install

In Claude Code:

```
/plugin marketplace add OneLeoTav/leotav-skills
/plugin install critical-thinking@leotav-skills
```

Then just start arguing — it triggers on phrases like *"challenge me on this,"* *"what's wrong with this argument,"* *"steelman this,"* *"poke holes in this,"* or *"stress-test this strategy."* Or invoke it directly:

```
/critical-thinking:critical-thinking
```

To update later:

```
/plugin marketplace update leotav-skills
```

## Try it

Paste in a decision you're about to make, or an argument you believe, and say **"poke holes in this."** Watch it steelman you first, then find the crux you were avoiding.

Five things it does that a yes-man won't:

- **Steelman, then strike.** *"Poke holes in this go-to-market plan."* It rebuilds your plan in its strongest form first, then names the single assumption that sinks it — instead of nitpicking the easy stuff.
- **Find the crux.** *"Challenge me on this architecture decision."* It isolates the one load-bearing assumption the whole choice rests on, and surfaces the trade-off you were stepping around.
- **Catch the over-correction.** *"I'm changing this to fix a problem where the system does too little."* It flips the question — *"and now, can it do too much? how far?"* A fix that only models the failure you're correcting often overshoots the other way, and no one tests that direction.
- **Quantify a vague claim.** *"This change clearly improves quality."* It pushes back — *"compared to what, and by how much? If the effect is smaller than your measurement noise, it's a coin flip, not an improvement."*
- **Expose a self-cancelling argument.** *"We'll tighten the rule, and add an exception to cover the cases we'd lose."* It shows the two halves work against each other: the cases the exception is meant to save are the same ones the tightening removes.

## License

[MIT](LICENSE) · by [Léo Tavernier](https://github.com/OneLeoTav)
