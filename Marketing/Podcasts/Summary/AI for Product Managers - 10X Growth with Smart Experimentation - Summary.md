# AI for Product Managers: 10X Growth with Smart Experimentation — Comprehensive Summary

## Overview

This episode is a deep-dive masterclass on how AI has transformed A/B testing and product experimentation. The guest is **Fred de Toddaro**, described as "one of the world's most knowledgeable people on AI and experimentation," who works at **Cameon** (an experimentation platform). The host is **Aakash** (referred to as "Hakash" once in the transcript), who runs the AI for Product Managers podcast and newsletter.

The episode covers: the historical evolution of AI in experimentation, the four-step experimentation loop and how AI affects each step, machine learning techniques (AI targeting, multi-armed bandits, contextual bandits, opportunity detection), the generative AI wave (content generation, RAG assist, prompt-based/vibe experimentation), how to measure AI features themselves, common PM misconceptions, and a live demo.

---

## Guest and Host

- **Guest:** Fred de Toddaro — experimentation expert, works at **Cameon** (experimentation platform)
- **Host:** Aakash — AI for Product Managers podcast/newsletter host

---

## Sponsors Mentioned

- **Jira Product Discovery** (Atlassian) — discovery, prioritization, and roadmapping tool; used by Canva, Deliveroo, The Economist. URL: `atlassian.com/product-discovery`
- **AIPM Certification on Maven** — run by **McDad Jaffer**, product leader at OpenAI; 8-week live cohort-based course; co-taught with **Mo Ali**; 4.9 rating with 133 reviews; alumni from OpenAI, Shopify, Stripe, Google, Meta; discount code: **AA25**. URL: `maven.com/product-faculty`
- **Mobin** — world's largest library of real-world mobile and web app designs (Airbnb, Uber, Pinterest); 1.7 million users. URL: `mobin.com/acos`; 20% off first year
- **Maven (general)** — courses on AI prototyping for PMs, product sense for PMs, AIPM certification. URL: `maven.com/x/acos`

---

## The Four-Step Experimentation Loop

Fred frames all experimentation around a simple four-step cycle:

1. **Ideate** — Form an idea and an assumption: "If I release this feature, it will increase [metric X] because of [reason Y]."
2. **Build** — Build the experiment and its variations.
3. **Configure** — Set targeting (who sees the experiment), KPIs, and success metrics.
4. **Analyze** — Look at results, learn, iterate.

> "It's a simple loop. You iterate as long as you learn something with your experiments."

---

## How AI Affects Each Step of the Loop

### Ideate Phase — AI as Co-Pilot

- **AI's role:** Moderate. AI can suggest ideas when given context about the business, users, website framework, and past experiments.
- **Evolution:** Initially limited to content generation suggestions (post-2022). With GPT-4, AI can now take a page and generate meaningful product ideas.
- **UX Memory concept:** AI can query a team's entire historical experiment knowledge base and flag: "This idea has been tested before. Here are the results. Do you want to proceed?" This prevents duplication and surfaces learnings across teams.
- **Host's recommended practice:** Build a Claude or ChatGPT project loaded with context (past features shipped, reasons for certain messaging, observed metrics, screenshot of the current page) to generate higher-quality ideas.

> "The AI can also bring some context from history. I like to call it UX memory... the AI will pop up saying this thing has already been tested and here are the results."

**Summary for PMs:** Human judgment and product sense remain most critical here. AI is a co-pilot, not a replacement.

### Build Phase — AI as Primary Builder (The Biggest Bottleneck)

- **Historical problem:** Over the past decade, experimentation tools have tried (and largely failed) to democratize the build phase with visual editors. Most teams still depend heavily on developers who are already busy building roadmap features.
- **Consequence:** Teams only A/B test a minority of what they ship; they hold prioritization meetings just to decide which experiments are worth the build cost; then wait 1–2 sprints to see anything go live.
- **AI's impact:** Vibe coding (using tools like **Lovable**, **Bolt**, **Replit**, **Cursor**, **Windsurf**) took this to the extreme. Now prompt-based experimentation means anyone can take an idea to a live running experiment in minutes, not sprints.

> "AI is fully capable of going from an idea to a prototype in just a few hours. But the real question isn't 'Can you build it?' It's 'Should you build it?'"

- **Fred's key insight on vibe coding limits:** Prototypes alone can't tell you if a feature actually works. Users say they want something and then don't use it when it ships broadly.

> "I've seen it so many times. Users say they want something. When you show a prototype they like it. And once you launch it to everybody — nothing happens."

- **Prompt-Based Experimentation (PBX):** Cameon's solution — "iterative vibe experimenting." You go to your real live website, type a plain-language prompt describing a change, and the AI generates the variation (JavaScript + CSS) and wires up a real experiment — directly on the production site, not a prototype. It then goes live to real users.

**Fred's stat target:** Drop developer dependency from ~80% of experiments needing custom code to ~20%. That is Cameon's internal target for PBX.

### Configure Phase — AI Does Most of It, Humans Review

- **PM's role:** Bring business context the AI lacks — customer commitments, internal constraints, assumptions, definition of success.
- **Data scientist's role:** The "essential human mind in the loop." Challenges AI output, checks for data bias, validates plausibility of results, selects the right statistical model (frequentist vs. Bayesian vs. CUPED), ensures the right metrics are defined and measurable.

> "The PM, the data scientist have to work together to make sure that the business context is there, the constraints are known."

- **AI's role:** Identify patterns, suggest recommendations when an experiment is non-conclusive, automate configuration steps.

### Analyze Phase — AI Does the Basics, Humans Define the Framework

- AI can produce full summaries of what happened during an experiment.
- AI can automatically drill down by dimensions (device type, user segment, geography) to surface performance differences.
- **Prerequisite:** Humans must pre-define the right northstar metric, guardrail metrics, and secondary metrics. Without this, AI cannot help.

> "If you run an experiment you are not able to measure the success, well, the AI will not help you."

---

## Historical Waves of AI in Experimentation

### Wave 1: Machine Learning Wave (starting ~2016)

Key capabilities that emerged:

#### 1. AI Targeting
- **Purpose:** Predict individual user conversion intent in real time.
- **Mechanism:** As soon as a visitor lands, the AI scores them (e.g., likelihood to convert) based on their behavior — pages visited, products viewed, time spent.
- **Analogy:** "We try to replicate what a good salesperson does in a physical shop — reading body language, movement, what products you look at."
- **Application:** Instead of creating manual segments, you use the AI's score directly as your targeting criterion. Example: only show a 10% discount popup to users whose intent score suggests they need it to convert — don't waste it on users who would buy anyway.

#### 2. Multi-Armed Bandit Algorithms
- **Purpose:** Optimize for performance, not just learning. Gradually allocate more traffic to the better-performing variant as data accumulates.
- **Trade-off:** Less statistical accuracy because decisions are made on smaller samples — but speed is gained.
- **Best use case:** Media/publishing — when you need to know within a day which headline drives more clicks. You don't care about perfect accuracy; you want to push the best headline fast.
- **Traffic requirement:** Needs significant traffic (100k+ visitors/month) to work well.

#### 3. Contextual Bandit Algorithms
- **Purpose:** Personalization. Push variant 1 to users who prefer it, variant 2 to users who prefer that — learning and adapting continuously.
- **Difference from multi-armed bandit:** Multi-armed bandit finds the single best variant for all users. Contextual bandit finds the best variant for each individual user.
- **Result:** Essentially a fully personalized website where every user sees the experience best suited to them.
- **Best use cases:** E-commerce (personalized coupons — 10% vs. 20% vs. 30% for different users), personalized homepages, any product with large user bases.
- **Traffic requirement:** Needs even more traffic than multi-armed bandit because it must learn enough about individual behavior before making decisions.

#### 4. Opportunity Detection
- **Context:** ~80% of experiments fail to improve the target metric. Data analysts manually drill into results to find why and where opportunities exist.
- **What AI does:** Automates this drilling. When an experiment is non-conclusive or shows a downlift, the AI automatically segments the data and surfaces insights like: "This variation performs well for mobile device users. If you personalize for them, you could increase revenue."
- **Value:** Works at a scale humans cannot — too many data points to crunch manually.

> "Less than 20% of experiments are successful, meaning when you ship a feature, 20% of the time it will increase the metric you want. So you want to make sure you're still learning something from that 80%."

### Wave 2: Generative AI Wave (starting 2022, accelerating with GPT-4)

#### 1. Content Generation
- **What it is:** Take existing website content (headlines, banners, popup copy, CTAs), ask AI to generate alternative versions for A/B testing.
- **How it started:** Initially models were only good at text. Every tool (Notion, etc.) started adding "generate this content" features.
- **Example:** Providing a prompt like "give me a more fun version of this" or "generate a version of this that's more compelling for podcast listeners."

#### 2. RAG-Based AI Assist (Chatbot)
- **What it is:** An AI assistant built into the experimentation platform (RAG = Retrieval-Augmented Generation) that answers questions and helps users navigate complex decisions.
- **Use cases:**
  - "Which statistical method should I use for this experiment?" (Frequentist vs. Bayesian vs. CUPED)
  - Generating code snippets for feature flags and SDK implementations without reading documentation
- **Cameon's implementation:** Users describe their experiment context and the AI recommends a method (e.g., "Use CUPED because you have historical data on this metric — it will reduce experiment duration by two weeks").

#### 3. Prompt-Based / Vibe Experimentation (most recent)
- **Triggered by:** Vibe coding going mainstream (~9 months before recording).
- **What it is:** A user navigates to their real website inside the Cameon platform, types a plain-language prompt, and the AI generates a live, testable variation directly on the production site.
- **Demo walkthrough:**
  1. Create a new experiment "by prompt"
  2. Select website and page to optimize
  3. Website opens inside the tool with a chat-style panel on the right
  4. Type prompt (e.g., "change the default sorting option to price low to high")
  5. AI uses chain-of-thought reasoning: identifies the target element, determines required JavaScript/CSS changes, checks mobile accessibility, checks accessibility compliance
  6. Code is generated; variation goes live on the site
  7. Total time: ~2 minutes for a change that would normally take 3–4 weeks (mockup → designer → spec doc → sprint planning → development)

- **Input modes supported:**
  - Plain text prompt
  - Uploaded mockup/Figma file
  - Hand-drawn sketch (mouse drawing)
  - The AI asks clarifying questions when context is missing (e.g., "What kind of image do you want?")

- **What it can build:**
  - New UI elements that don't yet exist (add-to-cart buttons, quick view modals)
  - Popups and banners
  - Layout changes (2 products per row instead of 4)
  - Onboarding flows and feature tours
  - Notifications with contextual information

---

## Statistical Methods Explained

### Frequentist Statistics
- The default method used by ~90% of the market.
- Tells you if variant X improves a specific metric with statistical confidence.
- Traffic is split equally; you wait until sample size is reached to make a decision.

### Bayesian Statistics
- Gives you a probability: "Variant A has an 80% chance of being better than control."
- Two schools of thought — some prefer Bayesian, most use Frequentist by default.

### CUPED (Cup-E-D)
- A more advanced statistical method, particularly powerful for B2B with many returning users.
- Takes historical data as input — when you start the experiment, you already have two weeks of metric data pre-loaded.
- Result: Can get statistically significant results much faster than starting from scratch.
- Best for: B2B products and platforms with returning user bases.

---

## The Right Workflow for PBX at Scale

Fred's recommended approach for larger teams with designers and engineers:

1. PM uses PBX to generate a variation in ~2 minutes
2. Generate a simulation link (shareable preview of exactly what users will see)
3. **Designer reviews:** Check brand consistency, UI/UX quality — they see the real thing, not a mockup
4. **Engineer reviews:** Click into the JavaScript section and review the generated code directly
5. **Data team reviews:** Check that the right goals and metrics are configured
6. Hit "finalize" to ship the experiment live

> "Everything is built directly on your website. The designer will see exactly what your users will see when the experiment goes live. That makes a total change."

> "How many times have we seen a huge disconnect between the PRD, the Figma, and what actually gets shipped to production? This is really allowing you access to 'okay, this is what we're about to ship.'"

---

## How to Measure AI Features

Fred outlines a three-layer measurement framework for any AI feature:

### Layer 1: Usage / Adoption
- Are people actually using the feature?
- Beware: stopping at usage is the biggest mistake teams make. Usage alone tells you nothing about value.

### Layer 2: Outcome
- Is it solving the problem users came for?
- Are they completing more tasks faster?
- Are they activating more experiments?

### Layer 3: Experience
- Once live, collect direct user feedback.
- The "thumbs up / thumbs down" mechanic seen in all AI tools — the primary signal for answer accuracy and completeness.

### Cameon's PBX-Specific Metrics
1. **How many prompts it takes to create an experiment** — too many = something is wrong with AI output quality
2. **Time from first prompt to experiment live** — goal is minutes vs. days/weeks
3. **How often developers still need to step in** — internal target: drop from ~80% of experiments needing code to ~20%

### Cameon's Northstar Metric
- **Number of experiments running daily on the platform**
- Chosen because:
  - Simple to measure — no data scientist needed to access the metric
  - Understandable by anyone in the organization
  - A drop = churn signal; an increase = new customers or more users creating experiments
  - Every department can contribute: product (features that make it easier), customer success (helping customers get value), marketing (publishing benchmarks per industry)

> "Fast gets good quicker than good gets fast. Do not wait for the perfect feature. You ship early and you iterate until you reach your goal."

---

## Measuring RAG Systems (Technical Metrics)

Three core technical metrics Fred tracks before shipping any RAG feature at Cameon:

### 1. Accuracy (Faithfulness)
- Is the answer actually grounded in real documentation that exists?
- Bad example: User asks "How is traffic split in a bandit?" AI answers "Traffic is always split evenly across all variants" — that's wrong for multi-armed bandit and contextual bandit.

### 2. Relevance
- Does the answer actually address the user's question?
- Bad example: User asks "What are the different targeting options for feature flags?" AI responds "You need to create a new experiment" — completely misses the question.

### 3. Context Quality
- Was the retrieved documentation actually helpful and up-to-date?
- If the AI pulls outdated documentation or old release notes, something is wrong.

### LLM-as-Judge Method
Cameon's operationalization approach:
1. A primary LLM generates an answer to a user question
2. A secondary LLM (the "judge") generates 2–3 new questions based solely on that answer
3. If those generated questions closely match the original user question — the answer was relevant
4. Apply this pattern across accuracy, relevance, and context quality to build an automated eval suite

> "Use an LLM as a judge. The LLM will generate two or three new questions based on the answer provided by the first LM. If those questions are very similar to the original question, the relevance is there."

---

## Company Spotlight: Booking.com as the Gold Standard

Fred singles out **Booking.com** as the company doing experimentation best (deliberately avoiding the typical examples of Netflix, Airbnb, and Microsoft):

- Nothing goes live — website, app, mobile — without going through experimentation first
- Built a true culture of experimentation from the top down
- Tests virtually everything

> "They have built such a strong culture of experimentation. Nothing goes live into production whether you are shipping a feature on your website, your application, your mobile application — they do everything through experimentation."

---

## Recommended Experimentation Maturity Ladder

Fred's advice for companies not yet doing experimentation — go step by step:

1. **Start with feature flags** — safely push code to production with an on/off switch. You can observe behavior and roll back instantly.
2. **Progressive rollouts / targeted delivery** — ship to 20% of users or a specific segment. Learn from real usage, find complaints, improve before full release.
3. **Full A/B testing at scale** — once you have the process, add heavy experimentation to make data-driven decisions broadly.

> "Don't go all in from day one. Start simple. We did that step-by-step at Cameon ourselves."

---

## Three Biggest PM Misconceptions About Experimentation

Fred frames these as misconceptions rather than mistakes:

### Misconception 1: "Experimentation will slow down our delivery"
- Reality: It speeds things up. You release early versions, learn from real users, and iterate to the right feature faster — rather than spending months building the "perfect" feature before shipping.
- Harvard Business Review study cited: **Direct correlation between number of experiments run annually and revenue growth.**

### Misconception 2: "We don't have enough traffic"
- Reality: Teams regularly validate features with just 10 prototype users and assume that generalizes to all users — yet they worry about traffic for experiments. That's inconsistent logic.
- Also: the number of conversions (not just visitors) matters for sample size. More conversion events = faster results.

### Misconception 3: "We do product discovery, so we're fine"
- Reality: Discovery and experimentation are complementary, not substitutes.
- **Product discovery tells you what users say they want.**
- **Experimentation tells you what users actually do.**

> "Discovery gives you early signals. Experimentation tells you exactly what users do when they interact with that feature. You need both to get the full picture in production."

---

## Key Roles in the AI-Augmented Experimentation Process

| Role | Primary Responsibility |
|---|---|
| Product Manager | Business context, internal constraints, defining "what success looks like," idea generation |
| Data Scientist | Challenging AI output, checking for data bias, validating result plausibility, selecting correct statistical model, defining measurable metrics |
| AI | Generating variations, identifying patterns, suggesting configurations, automating analysis, surfacing opportunity detection |

---

## Actionable Takeaways

1. **Load AI with rich context before ideating.** Create a dedicated Claude or ChatGPT project with past experiments, shipped features, messaging rationale, and metrics. The better the context, the better the ideas.

2. **Think of AI targeting as a real-time salesperson score.** Use intent scores from ML models to show coupons and personalized experiences only to users who need them — not everyone.

3. **Use multi-armed bandit for time-sensitive, single-winner decisions** (media headlines). Use contextual bandit for ongoing personalization at scale (e-commerce, large user bases).

4. **Don't just measure AI feature adoption.** Always measure outcome (did it solve the problem?) and experience (was the AI's answer helpful/accurate?).

5. **Define your northstar metric before building an AI feature.** Tie it to overall business outcomes, make it understandable across all departments, and make sure it's actionable (not just revenue).

6. **Implement LLM-as-judge for RAG systems.** Track accuracy, relevance, and context quality with an automated eval suite using a secondary LLM.

7. **Start with feature flags, then progressive rollouts, then full experiments.** Don't try to go to full experimentation culture overnight.

8. **Ship the first version, not the perfect version.** "Fast gets good quicker than good gets fast."

9. **In larger orgs, use PBX to compress review cycles — not eliminate them.** Use simulation links to get designer/engineer/data sign-off on the actual production experience before launch.

10. **The 80% rule.** ~80% of experiments don't improve the target metric. Build processes (like AI opportunity detection) to ensure you're still learning from failures, not just measuring wins.

---

## Notable Quotes

> "AI has been the biggest driver of change in experimentation I've seen in my career. I can't believe more people aren't using AI-based experimentation today."

> "The hardest part of experimentation has always been the build phase."

> "With AI, anyone in the organization — HR, finance, product manager — could directly come up with an idea, provide a prompt, and have a running experiment in minutes and not anymore in a sprint or two sprints."

> "Vibe coding became mainstream like nine months ago and if you look at experimentation it changes everything because it means you can turn any idea into a running experiment just by prompting an AI."

> "The real question isn't 'Can you build it?' It's 'Should you build it?'"

> "I've seen it so many times — users say they want something, they like it when you show them a prototype. And once you launch it to everybody, nothing happens."

> "You will only really know if it works when that feature is going live to all your users."

> "Prompt-based experimentation sits right at the crossroads of vibe coding and experimentation — we call it iterative vibe experimenting."

> "Fast gets good quicker than good gets fast."

> "Product discovery will tell you what users say they want. Experimentation tells you what they actually do."

> "There is a direct correlation between the number of experiments you run annually and your revenue growth. The more you experiment, the faster you can grow."

> "AI is a game changer to becoming a company like Booking.com. You have no excuse at this point."

---

## Upcoming Content Mentioned

- A complete course on **AI Experimentation** (this episode's subject)
- A complete course on **AI Discovery** with **Teresa Torres** (separate episode, referenced as perfect companion content)
- Host's newsletter post with all tools, frameworks, and links referenced in this episode

---

## Tools and Platforms Mentioned

| Tool / Platform | Category |
|---|---|
| Cameon | Experimentation platform (Fred's company); offers PBX, AI targeting, contextual bandit, opportunity detection, RAG assist |
| Lovable | Vibe coding / AI prototyping |
| Bolt | Vibe coding / AI prototyping |
| Replit | Vibe coding / AI prototyping |
| Cursor | AI coding assistant |
| Windsurf | AI coding assistant |
| GPT-4 | LLM (OpenAI) — cited as the inflection point for generative AI in experimentation |
| Claude | LLM (Anthropic) — referenced as a tool for building context-rich AI projects |
| ChatGPT | LLM (OpenAI) — referenced for project-based context loading |
| Notion | Referenced as early example of content generation AI integration |
| Jira Product Discovery | Product discovery & roadmapping (sponsor) |
| Maven | Online learning platform (sponsor) |
| Mobin | Mobile/web design reference library (sponsor) |

---

## Companies Referenced

- **Booking.com** — gold standard in experimentation culture
- **Netflix, Airbnb, Microsoft** — typical examples of experimentation-mature companies (deliberately not chosen by Fred)
- **Canva, Deliveroo, The Economist** — Jira Product Discovery customers
- **OpenAI, Shopify, Stripe, Google, Meta** — companies where Maven AIPM course alumni work
- **Harvard Business Review** — source of study cited: direct correlation between number of annual experiments and revenue growth
