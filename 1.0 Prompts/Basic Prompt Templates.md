# RCTFC Prompt Framework

**R – Role:** Define the persona the AI should adopt.
**C – Context:** Give background about the problem or situation.
**T – Tasks:** List, step by step, what the AI should do.
**F – Format:** Specify the output structure (table, bullets, word count).
**C – Constraints:** Set limits: scope, tone, length, things to avoid.

## Example

**Role:** You are a senior Azure data architect.
**Context:** I'm designing a lakehouse for a healthcare client with GxP compliance; data arrives from 20 source systems.
**Tasks:**
1. Propose a layered architecture.
2. Map each layer to Azure services.
3. Flag compliance risks.

**Format:** A table (Layer | Service | Purpose), then 3 bullet-point risks.
**Constraints:** Under 250 words, no vendor outside Azure/Databricks, plain language for non-technical stakeholders.

Meeting minutes prompts
Role: Act as an executive assistant skilled at extracting decisions and actions from unstructured meeting notes.

Context: Below are rough notes from a [MEETING TYPE — e.g. leadership sync, cross-functional review, client call] on [DATE] with attendees: [LIST NAMES AND ROLES].

Task: Extract all decisions made, actions assigned, and open questions that still need resolution.

Format: Three sections — Decisions Made (bulleted) + Action Items (table: Action | Owner | Due Date | Priority) + Open Questions (numbered list). Flag anything ambiguous with [UNCLEAR].

Constraints: Extract only what is explicitly stated. Do not infer or add context. Language should be direct and scannable — not narrative.

[PASTE MEETING NOTES BELOW]


Role: Act as a communications specialist writing professional leadership messages.

Context: [SITUATION/EVENT] occurred on [DATE]. The stakeholder group is [AUDIENCE — who they are and how they'll likely react]. They have [HIGH/MEDIUM/LOW] awareness of the background.

Task: Write a professional communication from [SENDER ROLE] to this stakeholder group addressing this situation.

Format: Subject line + Opening (acknowledge situation, 1 sentence) + Context (what happened and why, 2 sentences) + What's being done (2 sentences) + Next steps (2 sentences) + Close. Under 200 words.

Constraints: Confident but not dismissive. No corporate clichés. Direct and human tone. Do not minimise the issue — address it head-on.


Prompt 1
You are a senior marketing strategist. I'm launching a [PRODUCT] for [TARGET AUDIENCE] in [MARKET]. Our brand tone is [TONE]. Create a campaign brief including: hook angle, 3 content pillars, 5 headline variations, and 2 CTAs. Format as a document I can share with my team.

Prompt 2
Based on this campaign brief: [PASTE BRIEF]. Generate 15 variations of the main post — 5 for LinkedIn (professional, insight-led), 5 for Instagram (visual, emotional), 5 for Twitter/X (punchy, provocative). Each under the character limit for each platform.

Prompt 3
Write 10 subject line variations for an email promoting [OFFER]. Test these hypotheses: 1) curiosity gap, 2) specific benefit, 3) social proof, 4) urgency, 5) question. Rate each 1–10 for predicted open rate and explain why. I'm targeting [AUDIENCE] in [INDUSTRY].

Prompt 4
Take this blog post and repurpose it into: 1 LinkedIn article hook, 3 tweet threads, 1 email newsletter intro, 1 YouTube script outline, 3 Instagram caption options, 2 WhatsApp broadcast messages, 1 podcast talking points list. Blog post: [PASTE POST]

Prompt 5
I've collected these 5 competitor blog posts: [PASTE EXCERPTS]. Analyze: What topics are they owning? What's missing that we could cover? What's their average content depth? Give me 10 content ideas that would outrank or outperform their current content.