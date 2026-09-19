# AI Prompt Injection & PII Leakage Testing Sandbox

A hands-on security testing exercise: a deliberately vulnerable AI support
chatbot, built to practice and demonstrate real prompt injection, PII
leakage, and access control testing techniques.

## What's here

- **security-sandbox.html** — the actual test target. A support chatbot
  with a hidden system prompt holding fake confidential customer data and
  a deliberately weak access rule (trusts any self-reported employee ID
  with no real verification).
- **FINDINGS.md** — the full write-up: methodology, four attack
  techniques tested, actual results, and defense-in-depth
  recommendations.

## Summary of results

Four attack techniques were run against the live chatbot: direct
instruction override, roleplay/jailbreak framing, access control bypass,
and social-engineering-style PII leakage. All four were unsuccessful,
full findings and one notable observation about a documentation-vs-
behavior gap are in [FINDINGS.md](./FINDINGS.md).

## Why this exists

Built to gain genuine, hands-on experience with AI security testing
methodology, not just theoretical familiarity, as part of ongoing GRC
and AI governance work.
