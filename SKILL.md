---
name: pre-design
description: Prepare design direction before starting a visual project, beginning a new design phase, resetting an existing tone, or creating a major object such as a page, component, slide, card, chart, or visual system. Establish the minimum brief, constraints, references, tokens, and practical verification criteria before implementation. Skip only tiny mechanical edits whose direction is already fixed.
---

# Pre-Design

Resolve high-rework decisions before implementation. Use the smallest amount of discovery that prevents the work from starting in the wrong direction.

## Codex operating rules

1. Inspect the request, conversation, references, relevant files, existing styles, assets, and project records before asking anything.
2. Never ask the user to repeat information already available.
3. Choose one path:
   - **Proceed:** intent and constraints are clear.
   - **Assume:** a missing choice is reversible and low-cost; state one concise assumption and proceed.
   - **Ask:** a missing choice would materially change structure, brand, content, accessibility, or scope; ask one concise question.
4. Do not turn a short task into a questionnaire. Ask only what changes the result.
5. Record the chosen direction compactly, then hand off to the applicable brand, format, or implementation skill.

## When to run

Run this skill for:

- a new project or product with visual decisions;
- the first design pass for an existing project;
- a redesign, rebrand, visual refresh, or new tone;
- a new page type, design system, template, or campaign;
- a major object such as a hero, navigation, dashboard module, card family, chart, slide system, poster, thumbnail, or document cover;
- work described as “design it,” “make it polished,” “set the tone,” “make it on-brand,” or similar.

For an object inside an established system, preserve the parent system and define only the object-specific role, content, states, and constraints. Do not reopen settled project-level decisions.

Skip full discovery for tiny mechanical edits such as a known color replacement, typo correction, or fixed-size export. Preserve the current direction and verify the requested change.

## Select the scope

Classify the work before planning it.

| Scope | What must be fixed |
| --- | --- |
| Project kickoff | audience, problem, core action, content model, brand relationship, platforms, constraints |
| Design kickoff | visual stance, hierarchy, layout logic, type, color, imagery, motion, responsive behavior |
| Tone reset | what remains, what changes, target impression, migration boundary, before/after success signal |
| Object pre-work | object role, parent context, content, variants, states, dimensions, interactions, edge cases |

Use the narrowest applicable scope. Escalate from object to project scope only when the requested object exposes a genuine system-level conflict.

## Build the minimum viable brief

Resolve these fields from available evidence:

```text
Scope: project / design / tone reset / object
Deliverable: format, platform, dimensions
Audience and context: who encounters it, where, and under what conditions
Job: what the viewer must understand, feel, or do
Content: required copy, data, assets, and priority
Existing system: reusable styles, components, patterns, and protected decisions
Direction: brand or one coherent visual stance
Constraints: technical, accessibility, legal, schedule, and content limits
Done when: observable checks that prove the result works
```

For small or well-specified work, compress the brief to:

```text
[scope/deliverable] for [audience] to [job], preserving [existing system], using [direction], done when [checks].
```

## Gather evidence before choosing a direction

Use evidence in this order:

1. current project files, brand rules, approved assets, and existing product behavior;
2. user-supplied references and exact copy;
3. comparable products or visual references, when needed;
4. conservative defaults only when evidence is absent.

Separate references into:

- **keep:** decisions that already work and must remain;
- **change:** the specific perception or behavior to improve;
- **avoid:** patterns that conflict with the product or feel generic;
- **unknown:** items that need a safe assumption or one question.

Do not copy a reference wholesale. Extract useful properties such as density, rhythm, contrast, type character, image treatment, and interaction behavior.

## Lock direction at the right level

If a brand exists, load its skill and current tokens. Brand rules outrank generic preferences.

If no brand exists, choose one coherent stance rather than mixing styles:

| Direction | Character | Typical fit |
| --- | --- | --- |
| Editorial | typographic, warm, image-led | curation, essays, galleries |
| Modern Minimal | precise, quiet, high-contrast | SaaS, dashboards, documents |
| Tech Utility | dense, functional, system-like | developer and data tools |
| Brutalist | raw, oversized, confrontational | campaigns and experiments |
| Soft Warm | gentle, welcoming, low-friction | education, health, lifestyle |

Lock only the decisions needed for the selected scope:

- hierarchy and primary action;
- background, surface, text, muted text, border, accent;
- display and body type roles;
- spacing density, grid, radius, and shadow policy;
- imagery/icon/illustration treatment;
- motion character and reduced-motion behavior;
- object states and variants when designing a component.

Do not create extra palettes, font families, variants, or abstractions without a demonstrated need.

## Handoff contract

Before implementation, leave a compact handoff another Codex instance can act on:

```text
Intent:
Preserve:
Change:
Direction:
Required content/assets:
Primary action:
States/variants:
Constraints:
Verification:
Assumptions or unresolved items:
```

Keep it short enough to guide implementation. For an existing project, use its current handoff or progress record rather than creating a parallel tracker.

## Implementation guardrails

Reject generated-looking defaults unless the brief specifically supports them:

- decorative purple gradients, cyan glow, gradient headings;
- emoji used as interface icons;
- repeated identical icon-card grids or cards nested inside cards;
- invented metrics, decorative charts, or fake testimonials;
- glass, blur, noise, or animation without a functional role;
- Inter or monospace everywhere as a substitute for typography decisions;
- unrelated placeholder illustration;
- every action styled as primary.

Prefer real content, restrained tokens, deliberate hierarchy, consistent icon families, and complete interaction states. For web UI, run `authentic-web-design` after this skill. For branded work, apply the brand skill before generic visual preferences.

## Practical verification

Verify the artifact at the level the user will experience it. Source inspection alone is not enough for visual completion.

### Universal gates

| Gate | Pass condition | How to check |
| --- | --- | --- |
| Intent | audience, purpose, and primary action are evident | five-second read or first-screen inspection |
| Hierarchy | importance is visible without explanation | blur/squint test and reading order |
| Coherence | type, color, spacing, imagery, and motion express one direction | compare representative screens/objects side by side |
| Content | real copy/data/assets fit without accidental overflow or fabrication | test shortest, longest, empty, and error content where relevant |
| Function | interaction, navigation, states, and accessibility work | keyboard, focus, contrast, reduced motion, target-size checks |
| Context | output works in its actual size, device, or medium | responsive browser, slide render, print/export, or target preview |
| Restraint | every prominent element has a purpose | remove-one-element test |

### Scope-specific gates

- **Project kickoff:** one representative end-to-end path is coherent; major pages or objects share the same system.
- **Design kickoff:** representative desktop and mobile/output-size views preserve hierarchy and rhythm.
- **Tone reset:** before/after comparison clearly shows the intended change while protected behavior and content remain intact.
- **Object pre-work:** default, hover/focus/active/disabled, loading/empty/error, and content extremes are covered when applicable.

If a gate fails, revise the weakest cause and verify again. Do not expose internal scoring. Report evidence using:

- `implemented locally`
- `validated by render, build, test, or static check`
- `verified in real UI or target output`
- `not verified: reason / next exact check`

The goal is fewer wrong-direction iterations and a result that can be judged in the real context of use.
