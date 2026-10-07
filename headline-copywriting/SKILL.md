---
name: headline-copywriting
description: Write hero headlines, subheads and positioning for landing pages, sales pages, ads or emails with a research-first process - pick one ideal customer, mine their exact words, write a positioning brief, mirror proven headline structures, then score options with a synthetic persona panel. Use whenever the user asks for a headline, hero section, tagline, subheadline, value prop, positioning, or "rewrite the landing page copy".
---

# Headline copywriting

A six-step process for hero headlines that people understand in five seconds. It came out of a real homepage rewrite: two rounds of "creative" headlines were rejected, and the round that won came from the steps below, in this order. Do not skip steps. Do not show the user headlines that skipped them.

Worked example used throughout: a tool for freelancers who sell AI product photos. The winning headline was **"Find gigs, send samples and get paid"**, a mirror of Dubsado's "Book clients, send contracts and get paid".

## Why headlines usually fail

- Most of the effort goes into design and a little into words. Write the copy first, design after the copy is approved.
- The headline is written from the model's taste instead of the customer's words. Words like "creative OS", "precision" or "measured" sounded good to the writer and were used by zero customers.
- The whole pitch is crammed into the headline (12 to 19 words: audience, product, category, logo). A headline carries ONE idea. The subhead explains.
- New structures are invented. Proven structures beat invented ones.
- Clever lines have no category word. In testing, "Hired at first sight" and "A sample makes it real" scored 0 to 6% comprehension.

## Step 1. Pick one ideal customer, and get it approved before any copy

Read everything the user has about their customers: notes, interviews, support tickets, sales calls, analytics, any existing positioning docs. If there are several possible audiences, lay them out side by side in a plain-English table, recommend ONE for this page, and get the user's approval.

## Step 2. Voice-of-customer mining

Collect 150+ verbatim quotes from the ideal customer, each with a source link: Reddit, YouTube comments, forums, reviews of competitors, job posts, and first-party support or sales messages (names stripped). Tip: reddit.com often blocks scripted fetches, so the pullpush.io and arctic-shift archives are useful. Every quote must be a literal substring of its source. No paraphrasing.

Output: `quotes.md`, plus a summary ranked by theme, the objections in their words, and a table of "words they use vs words we use". This step is good work for a subagent.

## Step 3. Positioning brief (April Dunford style)

One page:
- the one reader, and what they want
- what they do today instead (the real alternatives, including doing nothing)
- the 3 or 4 things only this product does (verify each one actually exists in the product)
- the value of those things in the reader's terms
- the category, in plain words
- the proof available, and the proof gap
- the story spine (the reader is the hero, the product is the guide)
- page structure and writer rules

End with the decisions the user must make. Get approval before writing copy.

## Step 4. Build a swipe file, then mirror it

Collect proven headlines (start with `references/SWIPES.md` and `references/PATTERNS.md`: 79 headlines with templates):
- Live hero sections of successful products in or near the reader's market. Across 35 SaaS, creator and freelancer sites, the median hero headline is 6 words, range 2 to 12.
- Classic direct response: swiped.co, swipefile.com, Victor Schwab's "100 Great Headlines", Caples, Ogilvy, Schwartz.
- Offers that already sell to this same reader.

Refresh the swipe file when the market is different from the one in the examples.

Writer brief (give it to a strong writing model as a subagent): 30 headline and subhead pairs. Headline 3 to 9 words, ONE idea, and each one names the exact swipe it mirrors (verbatim + source) and keeps its rhythm. Subhead 12 to 30 words. It must make clear what the product is and who it is for, in the reader's words, then say how the headline's promise happens. Do not open the subhead with a robotic definition like "X is software that...". If a line reads like a spec, rewrite it.

How the winning mirror worked: Dubsado's "Book clients, send contracts and get paid" became "Find gigs, send samples and get paid". It is a list of the reader's jobs, in their verbs, in order, ending on money.

## Step 5. Synthetic persona panel

A subagent plays 12 personas built from the voice-of-customer quotes (for example: beginners, experienced users, people switching from an older way of working, a skeptic, a mobile skimmer). They judge blind. For each persona and each option:
1. Headline ALONE: "What is it, and who is it for?"
2. Headline + subhead: the same question, plus click intent (1 to 10) and a gut reaction.

Score comprehension strictly against the ground truth: 0 to 2 for WHAT and 0 to 2 for WHO.

Combined score = 0.5 x (click / 10) + 0.25 x headline-alone comprehension + 0.25 x with-subhead comprehension.

Report the top 6 with scores, the main misreading of each, and verbatim reactions.

Caveats: one model plays every persona, so gaps under 0.03 are ties. When the subheads all state the category clearly, with-subhead comprehension evens out, so headline-alone comprehension and click intent decide.

## Step 6. Present

Show the top 4 with their subheads, scores, the swipe each one mirrors, what the panel taught, and an honest caveat (for example "click interest tops out at 5/10"). Give one recommendation. The user picks, and their pick beats the panel's #1. (In the worked example the user chose the panel's #6, which the panel had misread as "a marketplace like Upwork". The fix was to clear up that misreading in the subhead.)

## Body copy: the user's own words first

Researched body copy built from frameworks, voice-of-customer tables and checklists tends to read like documentation, not copy. In the worked example it was rejected as "unreadable, uninteresting". If the user has their own writing about the product (a post, a newsletter, a sales call transcript, a founder story), build every body section from their sentences, stories and numbers, near-verbatim, and only add connective lines in their voice. Show a short, clean page (headings and copy only, no notes or options) for review.

Frameworks decide the section order and each section's job, never the sentences. Every line earns the next: hook, tension, a picture, a turn. If a line could sit on any SaaS site, rewrite it.

## House rules for all copy

- Follow the user's brand rules (name spelling, tone, banned words).
- No em dashes. No staccato chains of fragments. No "It's not X, it's Y", "The result?", "unlock", "seamless", "elevate".
- No invented numbers, testimonials, income or ROI claims. No client names unless the user says they are public.
- Use the customer's words from the voice-of-customer table.
- Long-form method: `references/COPY-PLAYBOOK.md` (Shapiro structure, Dry tests, StoryBrand, Epiphany Bridge, the pre-publish checklist).
