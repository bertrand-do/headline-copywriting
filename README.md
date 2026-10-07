# headline-copywriting

A Claude Code skill for writing landing page headlines that people understand in five seconds.

It doesn't brainstorm clever lines. It runs a research-first process:

1. **Pick one ideal customer** and get it approved before writing anything.
2. **Mine their exact words.** Collect 150+ real quotes from Reddit, reviews, forums and support tickets.
3. **Write a positioning brief** in the style of April Dunford.
4. **Mirror proven headlines.** It includes a swipe file of 79 headlines from live SaaS homepages and classic direct response, with the template behind each one.
5. **Test with a synthetic persona panel.** Twelve personas judge each option blind, scored on comprehension and click intent.
6. **Present the top 4** with scores and one recommendation.

It came out of a real homepage rewrite. Two rounds of "creative" headlines failed. This process produced the winner, *"Find gigs, send samples and get paid"*, a mirror of Dubsado's *"Book clients, send contracts and get paid"*.

## Install

```bash
git clone https://github.com/bertrand-do/headline-copywriting.git
cp -R headline-copywriting/headline-copywriting ~/.claude/skills/
```

Then ask Claude Code: *"write a headline for my landing page"*.

## What's inside

| File | What it is |
|---|---|
| `headline-copywriting/SKILL.md` | The six-step process |
| `references/SWIPES.md` | 79 proven headlines, quoted verbatim, with sources |
| `references/PATTERNS.md` | The templates behind those headlines and when each one works |
| `references/COPY-PLAYBOOK.md` | Long-form landing page method: structure, subheads, CTAs, and a 13-point pre-publish checklist |

## License

MIT
