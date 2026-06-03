# Become a 10x PLG Practitioner Using AI (7 Real Workflow Examples) — Comprehensive Summary

**Podcast:** The Product Podcast
**Host:** Wes Bush (ProductLed)
**Guest:** Akash Gupta — author of the largest newsletter in product and growth (nearly 200,000 subscribers)
**Format:** Conversation + live screen-sharing/demos

---

## Overview and Framing

The episode argues that AI and Product-Led Growth (PLG) are the best combination in the current landscape. The discussion breaks into two distinct but equally important sides:

1. **AI in your job** — how AI makes you a more effective PLG practitioner personally
2. **AI in PLG itself** — how AI transforms each layer of the PLG flywheel (activation, pricing, model, expansion, GTM, data, team, strategy)

The central metaphor: become a "10x practitioner" so you have the time, creativity, and leverage to focus on the strategic PLG work.

---

## Part 1: AI In Your Job (The Left Side)

### The Core LLM Toolkit

Akash organizes LLMs into categories rather than treating them as interchangeable:

**General-purpose LLMs (Claude + ChatGPT)**

- Wes uses ChatGPT for everyday brainstorming; Claude for copy, landing pages, and emails
- Technique Wes uses: "blast all of them" on deep questions — send the same hard question to Gemini, ChatGPT, and Claude simultaneously, then compare the different perspectives. "It's like talking to five different people on how do you approach this problem."
- Akash's take: "Claude is literally better at everything than ChatGPT guys. So use Claude instead."
- ChatGPT advantage: better value/token economics — when a Claude thread gets long, credits burn fast and you hit the plan limit; ChatGPT is more forgiving on cost

**Sole Context LLMs (NotebookLM)**

- Best tool in this category: **NotebookLM** (Google)
- Use case: When you have all the information you need and don't want the model to hallucinate by going to the web, load all context into NotebookLM
- Example: writing a document for your exec team — you already have all the data, just need synthesis
- Note: NotebookLM has a confusing UX because it emphasizes the podcast-creation feature. Ignore that. Its real value is loading massive context without hallucination risk.
- Accessibility: If your company has Google Workspace, you likely already have access — no IT request needed

**Projects / Co-Pilot Feature (Claude Projects or ChatGPT Projects)**

- Akash calls this "your co-pilot" — a specific project you train with important personal/company data
- What to load in:
  - Performance reviews
  - 1:1 notes from your boss and skip-level
  - Emails and context from leadership (strategy, vision documents)
- Wes's use case: loaded team personality assessments (KBA assessment) for every team member, then uses the project as a "chief people officer" — asks things like "How could Wes and Akash work better together?" or "Akash raised this issue — how should I approach it?" and gets tailored, accurate responses
- Tradeoff: burns tokens faster; may require upgrading to Claude Max or a higher ChatGPT plan
- "Projects, I think, are a huge unlock."

---

### Workflow 1: AI Agents for Internal Processes

**Agent Platforms by Complexity (hierarchy)**

| Platform  | Complexity              | Notes                                               |
| --------- | ----------------------- | --------------------------------------------------- |
| Lindy     | Easiest                 | Good starting point for non-technical practitioners |
| Relay.app | Easy-Medium             | Good product, solid for PLG use cases               |
| Zapier    | Medium                  | More powerful than Lindy; Airtable in same bucket   |
| Make.com  | Medium-High             | "Basically as good as n8n"                          |
| n8n       | Most powerful / hardest | Best for marketing ops or technical people          |

"If you're a marketing ops person listening to this, then probably n8n is great for you." — Akash

**Use Case: Competitive Analysis Agent**

- Monitors competitor pricing changes and feature launches
- Pings you in Slack instantly when a change is detected
- Can be trained with your own pricing strategy context so the alert includes analysis vis-a-vis your strategy
- "It can analyze it vis-a-vis my strategy and it'll have my insights on my pricing strategy too."

**Use Case: The AI Executive Assistant (12-Agent EA)**

- Reference: Jacob Bank (CEO of Relay.app) built a 12-agent EA covering the work of a ~$1,200/month human EA
- Functions it handles:
  - Meeting briefs
  - Adding Gmail events to calendar
  - Following up from meetings
  - Summarizing meetings to Slack
  - Reminding guests to RSVP
  - Flagging unusual calendar events
  - Filtering out cold sales emails
  - Giving stats on your email
  - Summarizing newsletters
  - Auto-replying to simple questions
  - Scheduling tasks and prioritizing
- Akash's advice: even if you have a human EA, use agents to automate the routine tasks so the EA can focus on decisions — "go from just a regular EA to a 10x EA"
- Wes's tactic: ask your team every week, "What are you doing now that you could probably automate with AI?" — create a running list and tackle one automation per week

---

### Workflow 2: AI Agents for Marketing

Akash is direct: "I'm sorry marketers, but AI agents are coming for your job."

**Reference: Jacob Bank's 40-Person Marketing Agent Team**
The full list of agents Jacob has built:

- LinkedIn post drafter
- LinkedIn comment replier
- YouTube description generator
- YouTube script generator
- LinkedIn post writer
- LinkedIn lead enricher
- LinkedIn influencer post researcher
- LinkedIn post tracker
- LinkedIn comment helper
- Tweet tracker
- Bluesky monitor
- Blog post writer
- Blog post updater
- LinkedIn post writer for new blog posts
- SEO ranking tracker
- Feature launch tracker
- Integration tracker
- Newsletter subscriber management
- Unsubscribe request handler
- Lifecycle marketing onboarding
- Customer tracking
- Churn customer handling
- Event scheduling and reminders
- Cohort onboarding
- Slack discussion agents
- Partnership application review
- Partnership finder
- Cold emailing for new partners
- Integration monitoring

"You can just do everything these days in marketing with agents. There's a huge arbitrage opportunity right now for people who are using AI to do marketing."

**Reference: Alex Hormozi**

- Released 500 pieces of content per week for his $100M+ book launch (biggest non-fiction book launch ever)
- The lesson: "There's something to just doing a lot of marketing and tools like this will help you do it."

---

### Workflow 3: Dictation Tools

**Why dictation matters:**

- Good typists: ~100–120 words per minute
- Average speaker: ~200–220 words per minute
- Akash: ~280 words per minute
- "You can speak way faster" — so prompting via voice gives you better, more context-rich prompts
- Solves the "lazy prompt" problem — people tend to type one sentence but would naturally speak a full detailed prompt

**AI dictation tools:**

- **Super Whisper** — Mac OS only; Akash's recommendation
- **Whisper Flow** — possibly Windows-compatible (not confirmed in the episode)
- Note: "This is an app idea for one of you guys out there" — Windows-native AI dictation is a gap in the market

**How they're better than Apple dictation:**

- Auto-formats sentence structure, punctuation, paragraphs
- "It's like 100x better than Apple dictation"
- Allows you to dictate your prompt to Bolt or Claude while prototyping, dramatically speeding up the iteration loop

---

### Workflow 4: AI Prototyping Tools

"I feel like everybody should be doing prototyping all the time. Like instead of suggesting a feature idea, you just prototype it."

**Why prototype instead of write specs:**

- Forces you into specific details (thumbnail for video, autoplay behavior, etc.)
- More actionable for your team than written suggestions
- Reveals gaps in your thinking immediately

**Tools:**

- **Bolt.new** — Akash's primary recommendation; he built a full website with free tools and SEO articles using it; "I vibe coded last night and it just launched online"
- **Lovable** — strong alternative, also recommended
- **Magic Patterns** — good for frontend/design prototyping; does NOT handle backend
- **Base44** — best for full apps with backend logic

**Base44 story:**

- Started as a one-person company
- The founder built Base44 on Base44 (dogfooding)
- Sold for $80 million all cash
- "If you want to build an $80 million solo person company, check out Base44."

**Live demo in the episode:**
Akash takes a screenshot of ProductLed's website and prompts Bolt to create a version with a "left-right top hero" layout (current left side + video sales letter on the right). The live result:

- Wes immediately sees he needs to think about YouTube vs. homegrown video player
- Notices the case study section should add Boomi and Zuzu logos
- Realizes the headline text is too long and needs tightening
- Dictates all these refinements to Bolt via Super Whisper in one voice prompt

"After just a few minutes, we'll have a nice prototype that you can send over your team that's like 10x more actionable than just you saying 'Hey, add a video.'"

**Bolt vs. Webflow/WordPress:**

- "The Bolt website is 100 times better. On those websites I couldn't have created these tools that I created."
- Tools built in Bolt can tap into LLM APIs, which is impossible in traditional CMS platforms

---

## Part 2: AI In PLG (The Right Side)

### Layer 1: Activation

**The core insight: Time-to-Value can be 1/10th of what it was**

Example from Akash's time as VP of Product at Apollo.io ($2.5B sales tech company):

- Old activation moment: user downloads an email from the contact database, then sends it
- With AI: when you log in, the system detects your domain (e.g., akash@news.ac.com), looks at your website, and immediately says:
  - "I think these 10 contacts you should reach out to are..."
  - "I think these would be really good podcast guests for you because I saw you're running a podcast. So I've also drafted these podcast emails for you."
- "That's how you deliver one-tenth the time to value."

**New Activation Metric Ladder:**
Old framework (setup + habit) is evolving. New ladder:

1. **AI-assisted activation** — the product does the work to get the user to the "aha moment" (1/10th TTV)
2. **User-driven activation** — the user has internalized the product and is activating themselves habitually

**Profiling for AI-assisted activation:**

- Wes: "The profiling questions are really really important to get the AI-assisted activation right. You ask the right questions, you can get way better AI-assisted activation. If you don't, then good luck. It could be hallucinating and not that helpful."
- Counter-trend: many companies are skipping profile questions entirely because they can infer from domain + enrichment tools (e.g., connecting to Apollo)

**AI Evals for activation:**

- When building AI features, you must have an AI eval suite
- Example eval for email-sending activation: Did they actually send the email? How many edits did they make? What types of edits did they make?
- Use an "LLM judge" to analyze edit patterns → feed that into your eval suite
- "AI evals are these really important thing when you're building AI features... that are going to assess the output"
- Goal: consistently measure and improve AI-assisted activation accuracy

**Recommendation:**

- "1/10th time to value is going to become the expectation in your market regardless of if you think it is possible or not. Somebody's going to figure out how to get people to value in one tenth of time. So best be you." — Wes

---

### Layer 2: Pricing

**The COGS problem:**

- AI features have real, significant cost of goods sold (COGS) — model inference is expensive
- Brian Chesky reference: Airbnb uses Alibaba's open-source Qwen model in production rather than OpenAI — "he says he doesn't even use OpenAI models in production"
- Key principle: use Claude/OpenAI in development; use cheaper/open-source models in production
- Build AI evals so your engineering team can optimize: "for a constant set of AI evals, how do we get the cheapest price?"

**The Pricing Hierarchy (moving from seats toward outcome):**

1. **Outcome-based pricing** (ideal)

   - Charge for results, not effort or usage
   - Examples:
     - **Finn (Intercom)** — Intercom had a $300M ARR business on traditional customer support software, then disrupted themselves with Finn: you pay only when AI resolves the customer complaint. "Outcome-based" canonical example.
     - **Harvey AI** (~$2–3B valuation) — charges per brief drafted or per contract reviewed, not per API call or seat
     - **Jasper** — charges per published blog post (not per generation)
     - **11x.ai** — charges per qualified meeting booked, not per email sent. Sales agent.
   - Benefit: "Somebody like Toyota might try you at 1%. And all of a sudden the outcomes work and they might just ramp you up all of a sudden."
   - Alignment: "Everybody in the company's like 'Hey, we need to book more meetings for our customers.' And it's like great. At the same time, we're making more money."
2. **Usage-based pricing**

   - Historical roots: AWS and infrastructure companies (forced to because they had to)
   - "The companies with the best margins and which grow most sustainably are those infrastructure companies"
   - Application-layer SaaS is now adding usage pricing for the same sustainability reasons
3. **Seat-based pricing with overages / multiple plans** (fallback)

   - The hack: charge overages when users exceed plan limits, and offer multiple plan tiers
   - Example: Claude's own pricing — regular plan users see "upgrade to Max" at thread limits; Wes burned credits so fast he defaulted to ChatGPT
   - Example: Warp.dev — set amount per plan, then charges overages
   - Example: Lindy — same overage model

**The decision framework:**

- "If you can define outcome, go for outcome. If you can define usage, go for usage. Otherwise, go for seats with overages and multiple tiers."

---

### Layer 3: Free Model Design

**Foundation: User research before free tier decisions**

- Map outcomes into 3 levels: beginner problems (whole TAM has these), intermediate milestones, advanced use cases
- Give away the beginner problems for free — "that's where I love to focus on that free model"
- Example from Vidyard: free = record video + send to anyone + see if they watched. Marketing analytics tools = the paid intermediate step.

**The Reverse Trial (now dominant for AI products):**

- COGS are high, but you need users to experience AI-assisted activation
- Solution: start users on a premium plan (reverse trial), let them use AI credits, then when credits run out: "You're out of AI credits — upgrade."
- "Before we used to give away so much... every month we would just refresh more and more and more credits. Now there is a cost."

**New model variations emerging:**

1. **Free trial with credit card** — more common now because of COGS; companies need some signal of willingness to pay
2. **Free trial with qualification** — e.g., require business email (not Gmail) to ensure enterprise intent
3. **Free plan without AI credits** — give the core product free, gate AI features behind payment (Cursor model)

**Cursor as a model case study:**

- Gives a genuinely good IDE for free with unlimited usage, but zero AI credits
- Millions of free users who pay for their own Claude Max to use Claude code inside Cursor Free
- "Create a free plan without AI" — let the AI spend fall on the user, not you

**The five ways to handle COGS in your free model:**
Akash lists these without fully enumerating all five in the transcript, but the discussion covers: reverse trial, credit-limited plans, free tier without AI, usage-based upgrades, and qualification-gated trials.

---

### Layer 4: Expansion

**AI-Assisted PQL (Product Qualified Leads) for expansion:**

Detailed example from Akash's time at Affirm (Director of Growth Product) with a product like Productboard:

- 100 PMs at a firm; 30 using the product well, 70 not
- Analysis shows: senior PMs are the most active users, not product leaders
- AI identifies: of the 70 non-users, 15 are senior PMs most likely to want the tool
- Next step: don't just target them generically — AI finds a specific customer insight relevant to each PM's current roadmap, then crafts a personalized expansion email referencing that insight
- "Do you see how powerful that is?"

**Impact on expansion metrics:**

- "Their expansion will go from let's say 110% as their average per year to 120%, 130%." — Akash

**Tools mentioned:**

- **Pocus** — PQL platform, building in AI-assisted expansion space

**How to implement:**

- Improve all existing triggers (transactional lifecycle emails, customer success calls)
- Layer in AI-assisted expansion signals at each touchpoint
- "You improve all of those with these AI-assisted expansions."

---

### Layer 5: Go-to-Market (GTM)

**Akash's observation:** GTM is "probably the area most disrupted by AI."

**Marketing side:**

- 10x more output is achievable right now; use the agent frameworks from Part 1
- Specific tactics:
  - **Webinars**: teams that didn't used to run webinars now can, because agents handle setup
  - **SEO at scale**: tool recommendation — **Outrank** — "will literally write an LLM-optimized article for you every single day, fully optimized for SEO with videos, images, infographics, FAQs, and backlinks from their marketplace"
  - **Employee LinkedIn**: most companies are under-indexed here; AI can now write all employees' LinkedIn posts and track performance at scale
  - **AI-generated video ads**: tools **VO3** and **Nano Banana** — companies like Lexus and Reebok are hiring specialist agencies to create viral ads with these; even small companies can now access this

**Sales side:**

- Finding leads + writing customized emails at scale
- **AI avatar companies**: Wes notes Vidyard is moving toward avatars; Akash shows a creator getting hundreds of thousands of followers per week using an AI avatar — recorded casual audio at his desk, AI generates polished video
- "If they're fooling millions of people every single day on Instagram... they definitely work."
- **Customized video outreach at scale** is now accessible

**AI email sequence optimization:**

- Old model: add 100 people to a generic sequence
- New model: add 5 people; embed tracking pixels; AI monitors opens, clicks, and what links they clicked on; uses those signals to analyze and iterate the email in real time; improves continuously
- "These are just amazing workflows. You can just get AI to do it all for you."

**Best sales tools:**

1. **Apollo** ("for sure")
2. **Instantly**
3. **Lemlist**

**The GTM gap:**

- Wes and Akash agree: no single tool gives you a unified view of your entire GTM motion (marketing + sales + CS in one place)
- Salesforce's marketing, sales, and support clouds are the closest thing
- Most high-performing teams use "17 different tools" with GTM engineers orchestrating them

---

### Layer 6: Data

**Current reality:**

- Most teams still do manual analysis: Wes says ProductLed uses Mixpanel, Amplitude, or PostHog depending on client budget, then analyzes the data themselves to identify bottlenecks

**Next-gen product analytics tools:**

- **Chameleon** — AI-forward product analytics
- **Statsig** — experimentation + analytics; "Statsig was just bought by OpenAI" — notable acquisition
- Legacy tools: Mixpanel, Amplitude, PostHog

**Advanced experimentation concepts:**

1. **Prompt-based experimentation:**

   - Instead of writing code to run an A/B test, you just hit "experiment" instead of "publish"
   - For frontend changes that don't touch the backend: send to on-call engineer, they review in 2 minutes, it's live
   - "That's what you can do with prompt-based experimentation nowadays."
2. **Bandit algorithms:**

   - Traditional A/B test: traffic allocated 50/50 until statistical significance
   - Bandit: as signal accumulates showing Variant A winning, algorithm continuously shifts more traffic toward A — faster convergence without ending the experiment early
   - Use case: "If you're doing a big marketing push or paying influencers to post about you, you want to make sure it doesn't take two weeks to shift to the winning variant."

**Data infrastructure approach:**

- Throw all data into a data lake or warehouse: **Ceso** or **Snowflake**
- With AI making SQL query writing trivial, you can connect 17 different data sources (CRM, WordPress marketing data, PQL data from Pocus, sales close/loss data from Salesforce) in one platform
- "AI making it so much easier to just write your SQL queries" removes the technical barrier to cross-source analysis

---

### Layer 7: Team

**The directional shift:**

- Teams are becoming "probably half the size across the board" — Akash
- The question to ask: "Do we have the right people in the right seats? Could that function be completely done by AI? Maybe not today, but in a year, absolutely."
- Rise of the **GTM engineer**: "the engineering of it all — once you set it up you can get 10x more output with a fraction of the team"

**Rethinking roles:**

- Content marketer example: the strategist who understands expertise is more valuable than someone who just writes content — AI handles the writing
- Even if you have a human EA, train them to use Relay, Lindy, etc., so they focus on decision-making, not logistics

**The agent org chart:**

- Wes: "That's a seat on the team. It's a vital function, vital job, but it's not human. It's the AI agent that's just going to be doing that."
- Inspired by Jacob Bank's model — design your org chart with agent "seats" explicitly labeled

---

### Layer 8: Strategy

**The commoditization thesis:**

- Features are now commoditized: "Taste is the differentiator." — Akash
- "SaaS is about to boom because there's a lot more micro SaaS out there" — contrary to common bearish takes

**Hard-to-copy moats:**

1. **Data** — proprietary datasets are extremely hard to replicate
2. **Distribution** — existing audience/customer relationships
3. **Taste** — the discipline of product craft

**What is taste?**
Akash's definition: "Taste is the ability to only show people what they need to see."

Examples:

- ChatGPT's homepage: just a blank white screen with a chat box. "They decided all they need to show you is a chat box. That's taste."
- Taste means giving people one or two things instead of a hundred
- "Creating a clearly sculpted journey through your product that layers in the right elements at the right time"
- **Zero tolerance for bugs**: "All your SaaS products out there listening are littered with bugs. Littered with bugs."

**Linear as the canonical taste example:**

- Just crossed $1 billion in revenue
- Product is task management — "you could probably vibe code the basic version in Bolt in 10 minutes"
- But Linear has zero tolerance for bugs: if a customer reports a bug, they solve it that day, even if only one person in the world has the issue
- "They're going to hit a billion and two billion and five billion and 10 billion sure enough, because they have that craft and taste."

**Live taste critique of ChatGPT:**
Akash tries to generate an image of himself speaking on stage; during the generation:

- No loading experience or progress indicator
- A 1:20 timer appears but doesn't reflect actual generation time
- "There's all these elements where just because a company is good at taste in one area doesn't mean they're always tasteful."
- Lesson: find the specific rough edges in your own product and eliminate them

---

## The Master Roadmap: Where to Start

### On the "AI in your job" side (pick one new tool per week):

Akash's recommended sequence for practitioners:

1. **Dictation** (Super Whisper) — most people aren't doing this, biggest immediate leverage
2. **Agents** (Lindy, Relay, Zapier, or n8n depending on technical comfort)
3. **Co-pilot project** (Claude Projects or ChatGPT Projects, trained with personal context)
4. **Prototyping tool** (Bolt.new or Lovable)
5. **Sole context LLM** (NotebookLM)

### On the PLG side (diagnose your weaknesses first):

- Honestly assess which of the eight layers you're weakest at
- Akash's example prioritization: "If you're pretty strong on activation, model, expansion, GTM, and data, but weak on team, strategy, and pricing..."
  - Team: do you have the right people using AI?
  - Strategy: have you built a hard-to-copy moat?
  - Pricing: are you stuck on seats? How do you move to usage? Stuck on usage? How do you move to outcome?

---

## How to Stay Current on AI

### Step 1: Follow the right people

**On X (Twitter):**

- **Andrej Karpathy** — "even his replies are packed with knowledge"
- **swyx** — runs the AI Engineering conference; "a legend"; posts amazing content
- **Greg Eisenberg** — "Are you following him? Are you checking out all his videos?" Including a 55-minute video on going viral on X

**On LinkedIn:**

- **Omninde** (Akash says "he is right at the top of my feed") — AI agent content
- **Reuben Hassid** — prompting and tools content
- **Jake Ward** — AI SEO content
- **Chris Donnelly** — entrepreneurship + AI; was ranking AI models during the episode

**On YouTube:**

- **Matt Wolf** — "Does the best job breaking down ChatGPT Atlas in a 30-minute video for you"
- **Nate Jones** — "The gray beard of AI. Really great, very high-value takes."
- **Peter Yang** — "Probably the most underrated channel for AI" — Claude code tutorials, Cursor tutorials, AI agent demos, "pretty sick beautiful designs"

**On Substack:**

- **Packy McCormick** (Powell Hearn)
- **Nicolas Cole**
- Both consistently writing about AI

### Step 2: Time-box tool trials

- When a new tool launches (e.g., ChatGPT Atlas), put it on the calendar: "15 minutes — try ChatGPT Atlas"
- If no major news-driven tool that week, pick one from your personal backlog list
- Akash's current backlog item: get better at make.com
- Resource: Lenny Rachitsky's Product Pass — gives access to ~30 tools with a list to work through

### Step 3: Mindset reframe

"Instead of thinking 'How do I stay up on AI?' or 'I'm feeling AI FOMO or somebody's beating me on AI' — think about 'How am I staying on the latest edge of technology?' And when you think about that, your answer will always be AI in the end." — Akash

"AI is just the better tool. It's the next evolution of technology. Do you guys remember when everybody switched from Outlook to Gmail? AI is just that." — Akash

---

## Key People, Companies, and Tools Referenced

### People

- **Akash Gupta** — Guest; largest PLG/product newsletter (~200K subscribers); former VP of Product at Apollo.io, Director of Growth Product at Affirm
- **Wes Bush** — Host; founder of ProductLed
- **Jacob Bank** — CEO of Relay.app; built 12-agent EA and 40-person marketing agent team
- **Alex Hormozi** — 500 pieces of content/week; biggest non-fiction book launch ever ($100M+ book)
- **Brian Chesky** — Airbnb CEO; confirmed using Alibaba's open-source Qwen model in production instead of OpenAI
- **Andrej Karpathy** — AI researcher; recommended to follow on X
- **swyx** — runs AI Engineering conference; recommended on X
- **Greg Eisenberg** — entrepreneur/creator; recommended on X
- **Omninde** — LinkedIn AI agent content creator
- **Reuben Hassid** — LinkedIn prompting/tools creator
- **Jake Ward** — LinkedIn AI SEO creator
- **Chris Donnelly** — LinkedIn entrepreneur + AI creator
- **Matt Wolf** — YouTube AI content creator
- **Nate Jones** — YouTube AI content creator ("gray beard of AI")
- **Peter Yang** — YouTube; "most underrated AI channel"; Claude code, Cursor, agent tutorials
- **Packy McCormick / Powell Hearn** — Substack AI writers
- **Nicolas Cole** — Substack AI writer
- **Lenny Rachitsky** — Product Pass gives access to ~30 tools

### Companies and Products

- **Apollo.io** — $2.5B sales tech; Akash was VP of Product
- **Affirm** — Akash was Director of Growth Product
- **Intercom / Finn** — canonical outcome-based pricing example; $300M ARR business disrupted itself
- **Harvey AI** — legal AI; $2–3B valuation; charges per brief/contract reviewed
- **Jasper** — AI content; charges per published blog post
- **11x.ai** — sales agent; charges per qualified meeting booked
- **Cursor** — AI IDE; free product, no AI credits; tens/hundreds of millions of free users
- **Warp.dev** — usage-based with overages model
- **Linear** — $1B revenue; zero bug tolerance; canonical taste example
- **Productboard** — used as PM expansion example
- **Vidyard** — free model: record and send video free; analytics = paid
- **ChatGPT (OpenAI)** — general LLM; Atlas version mentioned
- **Claude (Anthropic)** — general LLM; Max plan recommended
- **NotebookLM (Google)** — sole-context LLM; recommended for all PLG practitioners
- **Gemini (Google)** — mentioned; Wes doesn't use it regularly
- **Bolt.new** — AI prototyping/vibe coding; Akash built a full site on it
- **Lovable** — AI prototyping; recommended alongside Bolt
- **Magic Patterns** — frontend prototyping; no backend
- **Base44** — full-stack vibe coding platform; one founder sold for $80M cash
- **Relay.app** — agent platform; mid-complexity
- **Lindy** — agent platform; beginner-friendly
- **Zapier** — agent/automation; medium complexity; Airtable in same bucket
- **n8n** — most powerful agent platform; hardest to use
- **Make.com** — "basically as good as n8n"
- **Pocus** — PQL platform; building AI expansion features
- **Outrank** — AI SEO tool; writes daily LLM-optimized articles with images, infographics, FAQs, backlinks
- **Statsig** — product analytics + experimentation; acquired by OpenAI
- **Chameleon** — AI-forward product analytics
- **Mixpanel / Amplitude / PostHog** — standard product analytics stack
- **Snowflake / Ceso** — data warehouse for multi-source analysis
- **Salesforce** — closest to a unified GTM platform (marketing, sales, support clouds)
- **Apollo** — best sales tool for email sequencing
- **Instantly** — email outreach
- **Lemlist** — email outreach
- **VO3** — AI video/ad creation
- **Nano Banana** — AI video/ad creation
- **Super Whisper** — Mac OS AI dictation tool; recommended
- **Whisper Flow** — possible Windows dictation alternative (unconfirmed)
- **Qwen (Alibaba)** — open-source LLM; used by Airbnb in production
- **Lexus, Reebok** — mentioned as companies using AI-generated video ads

---

## Memorable Quotes

- "Claude is literally better at everything than ChatGPT guys. So use Claude instead." — Akash
- "You might be able to replace your EA at this point. Like AI has gotten so good." — Akash
- "There's a huge arbitrage opportunity right now for people who are using AI to do marketing." — Akash
- "I'm sorry marketers but your job — AI agents are coming for your job." — Akash
- "Features are now commoditized. Taste is the differentiator." — Akash
- "Taste is the ability to only show people what they need to see." — Akash
- "All your SaaS products out there listening are littered with bugs. Littered with bugs." — Akash
- "If they're fooling millions of people every single day on Instagram... they definitely work." [on AI avatars] — Akash
- "1/10th time to value is going to become the expectation in your market regardless of if you think it is possible or not. Somebody's going to figure out how to get people to value in one tenth of time. So best be you." — Wes
- "Instead of thinking 'How do I stay up on AI?' or 'I'm feeling AI FOMO' — think about 'How am I staying on the latest edge of technology?'" — Akash
- "AI is just the better tool. It's the next evolution of technology... Do you guys remember when everybody switched from Outlook to Gmail? AI is just that." — Akash
- "If you want to build an $80 million solo person company, check out Base44." — Akash [on the Base44 founder story]
- "What I would recommend is if you're listening to this on the podcast, definitely hop on to our YouTube channel at ProductLed where you can actually visualize a lot of the tools." — Wes [episode intro]

---

## Summary of the 7 Workflow Examples (Implicit from Episode)

While the episode doesn't formally number them, the seven core AI workflow categories for PLG practitioners are:

1. **Co-pilot / Projects** — train a personalized Claude/ChatGPT project with performance reviews, 1:1 notes, leadership context, and team personality data
2. **Agent automation for internal processes** — competitive analysis agent, 12-agent EA covering $1,200/month of EA work
3. **Agent automation for marketing** — 40+ marketing agents handling LinkedIn, YouTube, SEO, newsletter, partnerships, lifecycle
4. **Dictation-powered prompting** — use Super Whisper to speak prompts at 200–280 WPM instead of typing at 100–120 WPM
5. **AI prototyping** — vibe code website mockups, feature prototypes, and even full product tools in Bolt.new or Lovable instead of writing specs
6. **Sole-context LLM for synthesis** — use NotebookLM when you have all the data and need hallucination-free document generation
7. **AI-assisted PQL and expansion** — identify non-users within existing accounts, generate personalized use-case emails, and automate expansion triggers using tools like Pocus
