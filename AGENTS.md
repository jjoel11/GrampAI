# AGENTS.md

## Project Summary

GrandpAI is a lightweight app for grandparents to check a message, forwarded tip, or ChatGPT-generated idea before sending it to their kids or grandkids' parents.

Core purpose:

- help users sound supportive instead of intrusive
- help users avoid forwarding "helpful" AI output that creates more work for tired parents
- reduce guilt, pressure, unsolicited advice, and over-texting
- encourage concrete, caring actions when those are better than sending advice
- protect family relationships by making messages calmer, shorter, and kinder

The product should feel playful, but the underlying job is serious: help people communicate in ways that are helpful, not hurtful.

Primary product wedge:

- grandparents may use ChatGPT to generate ideas, scripts, advice, or lists
- instead of forwarding that output directly, they should run it through GrandpAI first
- GrandpAI should coach whether to send it, rewrite it, wait, or do something more useful in real life
- whenever appropriate, prefer practical help over another paragraph

## Primary Audience

The main user is a grandparent who means well and may not realize how a message lands.

Design and writing should assume:

- older users may prefer larger text, simpler layouts, and obvious controls
- the user should never feel mocked, scolded, or technically overwhelmed
- clarity beats cleverness when the two conflict

## Product Principles

- Be helpful first.
- Do not encourage emotional manipulation.
- Do not reward guilt, pressure, or repeated follow-up behavior.
- Favor warmth, brevity, patience, and respect.
- If a message would likely escalate tension, the app should say so plainly.
- If the best advice is "do not send this" or "wait", the product should be willing to say that.

## Brand Voice

Voice guidelines:

- affectionate
- honest
- lightly teasing
- plainspoken
- emotionally safe

Avoid:

- cruelty
- snark aimed at the user
- therapy jargon
- startup jargon
- overly technical product copy

The humor should feel like a knowing family wink, not a roast.

## UX Guidelines

- Prefer large, readable type and strong contrast.
- Keep navigation shallow and obvious.
- Use short labels and direct calls to action.
- Make the page easy to scan on both phones and desktops.
- Avoid clutter, dense dashboards, and tiny UI controls.
- Explanations should be in plain language.

## Messaging Guidelines

When generating examples, feedback, or rewrites:

- identify when a message sounds guilt-inducing, overbearing, repetitive, or too long
- identify when a forwarded ChatGPT answer sounds like homework, unsolicited advice, or extra emotional labor
- explain the issue in simple human terms
- offer a rewrite that sounds calm, respectful, and supportive
- when fitting, suggest a better non-text action such as bringing food, offering a ride, helping with errands, or simply waiting
- prioritize consent and space over unsolicited advice
- prefer short rewrites over long speeches

Good outcomes:

- "thinking of you"
- "happy to help if you want"
- "no pressure"
- "just checking in"
- "want me to bring breakfast"
- "I can drop groceries off if that would help"

Bad outcomes:

- "why have you not answered"
- "I told you already"
- "you should"
- "I am only trying to help" used as guilt
- forwarding a full ChatGPT list when one practical offer would be kinder

## Implementation Guidance

Until a fuller app stack exists, keep the codebase simple and easy to open locally.

Current repo expectations:

- root-level static files are acceptable
- prioritize readable HTML and CSS
- keep dependencies minimal unless there is a clear product need

If the app grows:

- preserve the warm, accessible visual language established on the landing page
- keep copy consistent with the "helpful, not hurtful" promise
- prefer straightforward flows over feature-heavy complexity

## For Future Agents

Before making changes:

- read `README.md`
- read `AGENTS.md`
- inspect the current landing page and any newer app entrypoints

When choosing between options:

- pick the one that is easier for a grandparent to understand
- pick the one that reduces the chance of hurtful communication
- pick the one that turns abstract advice into concrete help when possible
- pick the one that keeps the joke gentle rather than mean

If introducing AI analysis features:

- never frame manipulative language as effective
- never optimize for winning arguments
- optimize for kindness, restraint, and relational safety
- do not treat ChatGPT output as automatically good just because it sounds polished
- reward suggestions that replace advice-dumping with practical care
