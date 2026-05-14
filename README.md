# Journey Mapping

**A Claude plugin for building structured, research-grounded user journey maps.**

Intake to rendered HTML artifact — in one session.

---

## Install

1. Download `journey-mapping.plugin` from the [latest release](https://github.com/binkybink1/journey-mapping/releases/latest)
2. Open Claude Code → Settings → Plugins → Install from file
3. Select `journey-mapping.plugin`

---

## How it works

The plugin runs as a three-skill pipeline — always in this order:

**1. Intake** — a focused conversation to establish persona, scenario, map type, and what you actually know vs. what will be inferred. Takes 2-5 minutes. Never skipped.

**2. Data model** — generates a validated JSON object: the structured source of truth for the map. Every pain point and opportunity is tagged as `research`, `stated`, or `assumed`. You can review and edit before rendering.

**3. HTML render** — takes the JSON and produces a polished, fully self-contained HTML file with a stage-by-stage matrix, SVG emotional curve, and insights panel. No external dependencies. Works offline.

---

## Start a map

Just say what you want:

```
Map the onboarding journey for a new SaaS user
```
```
Create a journey map — I have a persona doc and some interview notes
```
```
I want to map the AEC preconstruction phase for a project owner
```

If you have existing artifacts (persona docs, empathy maps, research syntheses, interview transcripts, support tickets), paste or attach them. The plugin extracts aggressively and won't re-ask what your artifacts already answer.

---

## Map types

| Type | Use when |
|---|---|
| Current state | Documenting what actually happens today |
| Future state | Designing the aspirational experience |
| Day-in-the-life | Showing full daily context beyond a single product |
| Service blueprint | Adding the organizational backstage (frontstage + backstage + line of visibility) |

---

## Industries supported

The plugin detects your domain from context and selects the right stage library automatically.

| Industry | Stages |
|---|---|
| SaaS | Awareness → Consideration → Sign-up → Onboarding → Activation → Retention → Expansion → Advocacy |
| AEC | Inception → Planning & Design → Preconstruction → Construction → Commissioning → Post-Construction → Operations |
| Film/TV | Development → Pre-Production → Production → Post-Production → Distribution → Marketing → Exhibition |
| General | Awareness → Consideration → Decision → Usage → Loyalty |

---

## Confidence levels

Every map ships with a confidence badge:

- **High** — mostly research-based, backed by provided data
- **Medium** — a mix of research and inference
- **Low** — mostly AI-generated, limited real data

If you have almost nothing to work from, the plugin tells you before generating. A low-confidence map has value as a starting hypothesis — but only if everyone knows that's what it is.

---

## What the output looks like

The rendered HTML has three zones:

- **Zone A** — persona card, scenario, scope, map type, confidence badge
- **Zone B** — stage-by-stage matrix: actions, touchpoints, thoughts, emotional curve (SVG), pain points, opportunities
- **Zone C** — insights panel: top pain points, top opportunities, recommended focus

Open it in any browser. Screenshot it, drop it in Notion, share in Slack, present in a meeting.

---

Journey Mapping Plugin v1.0 — built for product managers and UX practitioners.
