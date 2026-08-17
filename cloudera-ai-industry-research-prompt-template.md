# Cloudera AI Industry Research System — Reusable Prompt Template

**Built for:** Sue Dunnell, PMM, Cloudera (CDE, CDW, CWO, OpDB)

**Purpose:** A repeatable prompt you paste into a Claude conversation to run a fresh deep dive, refresh an existing one, or turn findings into content ideas.

## How to use this

There are three prompts below. Prompt 1 is for a brand new industry or topic you haven't researched yet. Prompt 2 is for refreshing a topic you've already researched, so it only surfaces what's genuinely new. Prompt 3 turns any research output into webinar and content ideas. Run Prompt 1 once per industry or theme. Then run Prompt 2 on whatever cadence makes sense, monthly is reasonable, or on demand when something like the AI agent query cost story breaks. Each time you run Prompt 2, paste in the summary from the last run so Claude can tell you what changed rather than repeating itself.

Keep a single running log document, in your Google Working Doc or vault, with one dated entry per run. That log is what you paste back in as "previous findings" each time you refresh. This is the mechanism that gives you a memory system across sessions, since Claude itself doesn't retain state between separate research runs unless you're in the same conversation or I search past chats.

Fill in the bracketed fields before pasting.

---

## Prompt 1: New Industry Deep Dive

You are supporting me as a Product Marketing Manager at Cloudera, covering Cloudera Data Engineering, Cloudera Data Warehouse, Cloudera Workflow Orchestrator, and Operational Database. I need a deep dive on how organizations in [INDUSTRY OR SEGMENT, e.g. telecom, financial services, healthcare payers] are trying to use AI to solve real business problems right now, where they're getting stuck, and where the openings are for Cloudera to help them differentiate.

Research and report on the following, using current sources, industry reports, earnings calls, analyst commentary, vendor case studies, and credible practitioner discussion from the last six to twelve months:

One, the two or three business problems this industry is actually trying to solve with AI right now, stated in business terms, not technology terms.

Two, the specific pain points getting in the way, with a focus on data infrastructure issues: cost and unpredictability of running AI workloads against existing data warehouses and lakehouses, governance and data quality gaps, hybrid and multi-cloud complexity, latency or scale limits, and skills gaps. Cite sources and, where possible, quantify the pain, cost overruns, delayed timelines, failed pilots, with real figures.

Three, what "good" looks like, meaning what separates the organizations succeeding with AI in this industry from the ones stuck in pilot purgatory.

Four, where the competitive landscape sits: how are Databricks, Snowflake, and Greenplum positioning themselves for this industry's AI use cases, and what gaps or overclaims exist in that positioning that Cloudera's hybrid, multi-function platform story could credibly fill.

Five, three to five unique differentiators this industry's buyers should be pushing their vendors on, framed as questions a smart buyer would ask, not as a Cloudera pitch.

Format the output as plain prose organized under those five numbered sections, no markdown bullets or bold text, since I'll be pasting this directly into a working document. Cite sources by name inline rather than footnotes. End with a short list of the specific sources or reports that would be worth monitoring going forward for this industry.

---

## Prompt 2: Delta Scan / Refresh

I'm refreshing research on [INDUSTRY OR SEGMENT] that I last ran on [DATE]. Below is my previous findings summary. Your job is not to repeat this, it's to tell me what's actually changed or newly emerged since then.

[PASTE PREVIOUS FINDINGS SUMMARY HERE]

Search for developments from the last [30/60/90] days on this industry's AI adoption challenges, data infrastructure pain points, and vendor positioning from Databricks, Snowflake, and Greenplum. Report only on what is new or materially changed versus what's pasted above: new data points, new incidents or stories (like the kind of viral cost-overrun story that hits data warehouse bills), new analyst positions, new competitive claims, or a pain point that's clearly intensifying or fading. If nothing meaningfully new turned up, say so plainly rather than restating old findings. Flag anything that looks like a timely hook for a blog post, social post, or webinar. Plain prose, no markdown formatting.

---

## Prompt 3: Content and Webinar Ideation from Findings

Using the research below, generate content ideas for a PMM audience of technical buyers and IT decision makers in [INDUSTRY OR SEGMENT].

[PASTE RESEARCH FINDINGS FROM PROMPT 1 OR 2 HERE]

Give me five content ideas spanning at least one webinar, one blog or thought leadership piece, and one shorter format like a LinkedIn post or short video. For each idea, give me a working title, the specific pain point or finding it's built on, the audience it's aimed at, the single hook or tension that would make someone click or register, and a one-sentence angle for how it connects to Cloudera's actual capabilities without turning into a product pitch. Favor ideas built around a real tension or surprising data point over generic "AI and data" framing. Note which idea has the most urgency, meaning which one ties to something happening in the market right now versus which one is evergreen. Plain prose, no markdown bullets or bold text.

---

## Notes for Keeping This Current

If you want this to run without you manually re-prompting each time, Claude Cowork supports scheduled recurring tasks, you describe the job once, set a cadence, and it delivers results on its own. That would mean handing Prompt 2 to Cowork as a standing weekly or monthly job pointed at your running log. Worth trying if you find yourself re-running Prompt 2 often enough that the manual trigger becomes the friction point.
