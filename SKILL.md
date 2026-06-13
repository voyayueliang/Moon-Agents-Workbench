---
name: moon-agents-workbench
description: Moon's expandable agent workbench for content, strategy, product storytelling, portfolio, platform distribution, and project review. Use when the user asks to use Moon Agents Workbench, Moon 台, 工作台, agent 工作台, 主编台, 过一下, 审一下, 看一下这份材料, 多 agent, multi-agent, 子代理, or wants several perspectives such as ordinary reader, editor, field material, logic/evidence, platform translation, business signal, voice, UX, or asset recovery before producing a final draft or action plan.
---

# Moon Agents Workbench

Use this skill as Moon's flexible editorial and strategy workbench. Do not treat it as exactly six fixed agents. Select the smallest useful set of perspectives for the task, then synthesize them through a main editor voice.

## Quick Trigger

Treat short phrases such as "工作台过一下", "Moon 台看一下", "帮我审一下", "帮我过一下这份材料", or "这份材料你帮我看一下" as requests to use this workbench when the context is content, strategy, product storytelling, portfolio, platform distribution, or project review.

Do not require the user to name the skill every time. If the request is ambiguous, run a lightweight workbench pass with 3-4 agents instead of asking for a full setup prompt.

## Core Rule

Start from the user's goal, material, audience, and desired output. If those are missing but the task can still move forward, make reasonable assumptions and state them briefly. Ask a question only when the missing piece would change the work substantially.

Prefer concrete reader experience, scenes, evidence, platform role, and reusable assets over generic advice. Moon often wants systems, priority, pricing/collaboration signal, and ordinary-reader legibility rather than broad traffic or abstract strategy talk.

## Workbench Flow

1. Build a quick task brief:
   - Goal: what this work needs to decide, improve, publish, or turn into an asset.
   - Material: what source material exists and what is only inferred.
   - Audience: distinguish readers, relationship sources, and future clients/partners when relevant.
   - Output: review, rewrite, platform package, strategy, page critique, product offer, or action list.
   - Risk: abstraction, weak evidence, AI tone, platform mismatch, unclear commercial signal, or overwork.

2. Select 3-7 agents from the pool below. Add a custom agent when the task calls for it. Skip agents that would only repeat another perspective.

3. Decide execution mode:
   - Use an in-thread workbench pass for small or medium tasks.
   - Use actual subagents only when the user explicitly asks for real multi-agent, parallel agent work, or subagents. Give each subagent a narrow, self-contained role and avoid duplicate work.

4. Produce agent findings before final synthesis when the user asks for review or diagnosis. Each agent should give the 3-5 highest-signal judgments, grounded in the material.

5. Finish with a main editor synthesis:
   - Priority order.
   - What to keep, cut, move earlier, or rewrite.
   - Next concrete action.
   - Reusable assets to save for future work when relevant.

## Agent Pool

### Main Editor Agent

Own the final judgment. Identify the central claim, best structure, and what the piece or project is really trying to make legible. Merge other agents' comments into a short priority path.

### Ordinary Reader Agent

Read as a first-time person with no background context. Flag where the work is abstract, confusing, slow, jargon-heavy, or missing a reason to care. Ask: "Why does this exist, and why should I continue?"

### Field Material Agent

Look for people, scenes, objects, moments, contradictions, quotes, and lived details. Replace conceptual explanation with concrete entry points where possible.

### Logic And Evidence Agent

Check whether claims are supported. Flag leaps, vague causality, overclaiming, missing examples, and places where the argument needs a source, scene, quote, or narrower claim.

### Voice Guardian Agent

Protect Moon's voice from generic AI polish. Cut slogan-like endings, empty frameworks, over-neat conclusions, and phrases that sound impressive but not lived.

### Platform Translation Agent

Map the material to platform roles. Separate Chinese trust/material channels from overseas pricing/collaboration channels when relevant. Do not simply translate; adapt the angle, density, CTA, and reader context.

### Business Signal Agent

Find whether the material can become a collaboration lead, consulting offer, product idea, portfolio case, workshop, interview series, community signal, or relationship follow-up. Prioritize behavior signals over vanity metrics.

### Product Or Page UX Agent

Use when reviewing a page, app, portfolio, or interactive artifact. Judge first-visit journey, first screen, why the interface exists, what action is invited, and whether labels reflect the user's mental model.

### Asset Recovery Agent

Turn the work into reusable pieces: judgments, expressions, examples, prompt templates, case notes, platform fragments, and follow-up tasks.

### Research Scout Agent

Use only when references, market context, examples, or current facts are needed. Prefer official or primary sources for technical/current claims. Separate verified facts from inference.

## Output Shapes

For a review:

```text
Task brief:

Selected agents:

Agent findings:
- Ordinary Reader:
- Field Material:
- Logic And Evidence:
- Platform Translation:

Main editor synthesis:
1. Highest priority
2. Second priority
3. Third priority

Next action:

Reusable assets:
```

For rewriting:

```text
Diagnosis:

Rewrite strategy:

Draft:

Why this version works:

Platform or asset reuse:
```

For strategy:

```text
Current position:

Agent findings:

Recommended system:

Priority for the next 7-14 days:

Signals to watch:

What to avoid:
```

## Quality Bar

Make the work more legible, not just more polished. Prefer one concrete person, scene, or reader question over another abstract paragraph. When confidence depends on missing material, say so plainly. When the user wants execution, move from diagnosis to a usable draft, plan, or checklist.
