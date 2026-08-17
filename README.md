# leotav-skills

A [Claude Code](https://claude.com/claude-code) plugin marketplace with skills by [Léo Tavernier](https://github.com/OneLeoTav).

## Skills

### `critical-thinking`

A rigorous intellectual sparring partner — not an assistant, a thinking peer. It steelmans your position before critiquing it, hunts the one assumption the conclusion hinges on, and refuses to validate a claim just because you defend it. Built for debating a thesis, stress-testing a strategy, or poking holes in an argument.

What it does differently:

- **Anti-sycophancy by default** — agreement is earned with reasoning, never granted out of politeness.
- **Steelman first** — attacks the strongest version of your position, never a strawman.
- **Crux-hunting** — isolates the load-bearing assumption instead of nibbling at edges.
- **Output discipline** — leads with the punch, plain words for hard ideas, no filler. A 30-word reply can demolish a weak argument.
- **Calibrated intensity** — a casual question gets a sharp take and one destabilizing question; a developed argument gets the full analytical treatment.

It triggers when you say things like *"challenge me on this,"* *"what's wrong with this argument,"* *"steelman this,"* *"poke holes in this,"* or ask to stress-test a business strategy, philosophical position, or policy proposal.

## Install

In Claude Code:

```
/plugin marketplace add OneLeoTav/leotav-skills
/plugin install critical-thinking@leotav-skills
```

Then invoke it explicitly with `/critical-thinking:critical-thinking`, or just start a discussion and let it trigger on the phrases above.

To update later:

```
/plugin marketplace update leotav-skills
```

## License

[MIT](LICENSE)
