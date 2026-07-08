# SignalBrief

**Real-time social and market intelligence briefs for decisions that cannot wait.**

SignalBrief is a MiamiCreme rebrand and productization layer around the open-source `last30days` research engine. It turns scattered public signals from Reddit, X/Twitter, YouTube, TikTok, Instagram, Hacker News, Polymarket, GitHub, Perplexity, and the web into short, evidence-driven briefs.

> Search engines rank pages. SignalBrief ranks what people are saying, sharing, building, betting on, and reacting to right now.

---

## What SignalBrief Is

SignalBrief is a decision-intelligence workflow for founders, consultants, sales teams, recruiters, investors, operators, creators, and dealmakers.

Use it before you:

- take a sales or discovery call,
- research a company, founder, buyer, market, or competitor,
- validate a product idea,
- write outreach,
- prepare a client brief,
- compare tools or vendors,
- monitor fast-moving market sentiment,
- understand what real users are complaining about.

---

## Positioning

**Old positioning:** `/last30days` — an AI agent-led search engine scored by upvotes, likes, and real money.

**New positioning:** `SignalBrief` — real-time social and market intelligence briefs powered by what people actually engage with.

**Brand promise:** Know what the market is saying before you make a move.

---

## Primary Brief Types

| Brief | Purpose | Best For |
|---|---|---|
| Company SignalBrief | Company news, social chatter, hiring signals, founder activity, complaints, and competitor pressure | Sales, consulting, diligence |
| Founder SignalBrief | Recent posts, interviews, GitHub activity, controversies, interests, and talking points | Meetings, recruiting, partnerships |
| Competitor SignalBrief | Side-by-side market perception, feature chatter, complaints, strengths, weaknesses, and momentum | Product and strategy teams |
| Buyer Pain SignalBrief | Real user complaints, workarounds, buying triggers, and repeated pain language | SaaS, agencies, product builders |
| Deal SignalBrief | Public sentiment, local/community chatter, demand signals, risk notes, and outreach angles | Real estate and acquisition workflows |
| Trend SignalBrief | What is breaking, spreading, being debated, or monetized across communities | Creators, investors, researchers |

---

## Current Runtime Status

This repository is in the first rebrand pass. The inherited runtime command and skill path are still:

```bash
/last30days <topic>
```

```text
skills/last30days/SKILL.md
```

The next engineering pass should add a branded command while preserving backward compatibility:

```bash
/signalbrief <topic>
```

---

## Install During Rebrand

Until the command migration is complete, install from the fork and use the inherited command:

```bash
npx skills add miamicreme/signalbrief -g
```

Example runs:

```bash
/last30days OpenAI
/last30days "OpenAI vs Anthropic"
/last30days "Southern Tier Technologies" --hiring-signals
```

---

## Rebrand Roadmap

### Phase 1 — Brand Layer

- [x] Rename public README positioning to SignalBrief.
- [x] Define target users, use cases, and brief types.
- [x] Preserve upstream attribution.
- [ ] Add SignalBrief examples and sample outputs.
- [ ] Create a clean visual identity and repo social preview.

### Phase 2 — Compatibility Layer

- [ ] Keep `/last30days` as a legacy alias.
- [ ] Add `/signalbrief` as the preferred branded command.
- [ ] Rename user-facing output paths from `Last30Days` to `SignalBrief` with migration support.
- [ ] Update package metadata, marketplace metadata, and skill descriptions.
- [ ] Verify installs across supported Agent Skills hosts.

### Phase 3 — Productized Workflows

- [ ] Add saved brief templates.
- [ ] Add company, founder, competitor, buyer-pain, deal, and trend workflows.
- [ ] Add client-ready HTML brief themes.
- [ ] Add watchlists and recurring brief patterns.
- [ ] Package vertical versions for consulting, real estate, recruiting, and product research.

### Phase 4 — MiamiCreme Ecosystem

- [ ] Connect SignalBrief outputs to SkillForge playbooks.
- [ ] Add DealFlow-specific research templates.
- [ ] Add consultant discovery templates.
- [ ] Add outreach drafting workflows grounded in SignalBrief findings.

---

## Attribution

SignalBrief is based on [`mvanhorn/last30days-skill`](https://github.com/mvanhorn/last30days-skill), used under the MIT License.

The original project provides the core multi-source research engine, command behavior, setup flow, and source integrations. SignalBrief is a MiamiCreme rebrand and productization layer focused on clearer business positioning, repeatable decision briefs, and client-ready intelligence workflows.

---

## License

MIT. See [`LICENSE`](LICENSE).
