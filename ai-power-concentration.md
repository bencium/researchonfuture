# AI Power Concentration
## Why Intelligence Abundance Doesn't Mean Power Diffusion

---

## Executive Summary

**The core paradox**: AI promises to democratize intelligence, but the infrastructure to create and run frontier models is concentrating in fewer hands than any previous general-purpose technology.

**Why it matters**: If intelligence becomes abundant but computational infrastructure remains scarce, control over that infrastructure determines who benefits from the AI revolution—and potentially who survives it.

**Key dynamics**:
1. **Capital intensity** creates natural monopolies in AI development
2. **Prisoner's dilemma** forces competitive racing despite readiness concerns
3. **Substrate control** (energy, chips, data centers) becomes the new power base
4. **Intelligence vs. infrastructure**: Smarter AI doesn't automatically redistribute power

This article explores these dynamics, their historical parallels, and what they imply for the next decade.

---

## Part 1: The Gawdat Framework and Its Critics

### Mo Gawdat's Argument

Mo Gawdat, former Google X executive and AI researcher, has argued:

1. **Competitive pressure forces AI development** regardless of safety readiness (prisoner's dilemma)
2. **Current leadership is unfit** to steward transformative AI (his phrase: "evil leaders")
3. **AI could replace bad leaders** because intelligence itself is liberating
4. **Capitalism's profit-maximization logic** is the underlying problem

### What Resonates

**The prisoner's dilemma framing is compelling**:
- If Country A pauses AI development for safety, Country B races ahead
- If Company A self-restrains, Company B captures the market
- Rational individual choices → collectively terrible outcomes
- No Nash equilibrium at "slow down and coordinate"

**The social media critique lands**:
- Promised: Connection, community, information access
- Delivered: Isolation, performative tribalism, attention extraction, more work not less
- Same institutions deploying AI already optimized for addiction and engagement, not flourishing

### Where Critics Push Back

**Gawdat's optimism about AI replacing leaders is naive**, his critics argue:

If you accept his premise—that capitalism's profit-maximization is the core problem—then AI gets deployed **by that same system, for that same system**. The incentive structure doesn't magically change because the tool is smarter.

**The structural critique**:
- AI concentrates power because it's **capital-intensive**
- Training GPT-4 costs ~$100 million
- Training next-gen models (GPT-5, Gemini Ultra 2.0) estimated at $1 billion+
- Only massive entities can afford this: corporations or states
- Both optimize for control, not benevolence

**So the real question isn't**: "Will AI serve evil leaders?"
**It's**: "Does the architecture of power change when intelligence becomes abundant but computational infrastructure remains scarce?"

---

## Part 2: Capital Intensity and Natural Monopolies

### The Cost Curve

| Model | Year | Training Cost (Estimated) | Parameters | Company |
|-------|------|---------------------------|------------|---------|
| GPT-2 | 2019 | ~$50,000 | 1.5B | OpenAI |
| GPT-3 | 2020 | ~$4.6M | 175B | OpenAI |
| PaLM | 2022 | ~$10M | 540B | Google |
| GPT-4 | 2023 | ~$100M | ~1.76T (rumored) | OpenAI |
| Gemini Ultra | 2024 | ~$150M+ | Undisclosed | Google |
| Next-gen (GPT-5?) | 2025? | $500M - $1B+ | ? | OpenAI / others |

**Key observation**: Cost is growing **faster than Moore's Law improvements**.

Why?
- Model size scaling (more parameters = more compute)
- Data requirements (need massive, high-quality datasets)
- Infrastructure (custom chips, data centers, cooling, energy)
- Talent costs (top AI researchers command $1M+ salaries)

**This is not software's normal cost structure**:
- Typical software: High fixed cost (development), near-zero marginal cost (distribution)
- Frontier AI: **High fixed cost AND high ongoing cost** (inference at scale, fine-tuning, alignment)

---

### Historical Parallels: Capital-Intensive Infrastructure

**1. Railroads (1860s-1900s)**
- Required enormous upfront capital: land acquisition, track laying, locomotives
- Natural monopolies emerged: only 1-2 viable rail lines per route
- Concentrated wealth: Vanderbilt, Gould, Stanford
- Regulatory response: Interstate Commerce Act (1887), Sherman Antitrust (1890)

**2. Oil Refining (1870s-1911)**
- Standard Oil controlled 90% of U.S. refining by 1890
- Rockefeller's advantage: Vertical integration, economies of scale
- Infrastructure moats: Pipelines, storage, distribution
- Outcome: Broken up in 1911, but wealth already concentrated

**3. Semiconductor Fabs (1990s-present)**
- Modern fab costs: $10B - $20B per facility
- Only 3 companies can make cutting-edge chips: TSMC, Samsung, Intel
- ASML monopoly: Only supplier of EUV lithography machines (€350M each)
- Result: Chips are geopolitically strategic, Taiwan becomes critical flashpoint

**4. Cloud Computing (2000s-present)**
- AWS, Google Cloud, Azure dominate
- High capex: Data centers, custom chips (TPUs, Graviton), networking
- Economies of scale: More usage → better margins → more reinvestment
- Result: 67% of cloud infrastructure controlled by 3 companies

**Pattern**: Capital-intensive infrastructure with **economies of scale** → natural monopolies → concentrated control → eventual regulation (sometimes).

---

### Why AI Fits This Pattern

**Economies of scale**:
- Training one model costs $100M, but inference for millions of users amortizes fixed costs
- Data network effects: More users → more data → better models → more users (flywheel)
- Talent concentration: Best researchers want to work where compute is abundant

**Barriers to entry**:
- Can't build a GPT-4 competitor in your garage (unlike early web apps)
- Even well-funded startups (Anthropic, Inflection) need $100M+ in funding just to compete
- Open-source models (LLaMA, Mistral) lag frontier by 12-18 months

**Network effects**:
- Enterprise integration: Once Microsoft embeds GPT-4 in Office, switching costs are massive
- API ecosystems: Thousands of apps built on OpenAI API → lock-in
- User familiarity: "ChatGPT" becoming genericized term (like "Google it")

**Result**: Power law distribution. Top 3 labs (OpenAI, Google DeepMind, Anthropic) control frontier capabilities. Everyone else is 1-2 generations behind.

---

## Part 3: The Prisoner's Dilemma and Race Dynamics

### Game Theory Setup

**Players**: Countries, companies, research labs
**Choices**: Build AI fast (race) or slow down for safety (pause)
**Payoffs**:

|  | Rival Races | Rival Pauses |
|--|-------------|--------------|
| **You Race** | Tie (arms race), high risk | You win (capture value) |
| **You Pause** | You lose (fall behind) | Tie (safe, but low growth) |

**Nash Equilibrium**: Both race, even though mutual pause might be better.

**Why the dilemma is worse for AI than nuclear weapons**:

| Nuclear Weapons | AI Development |
|-----------------|----------------|
| Clear red line (detonation) | Gradual capability gains |
| Observable tests | Secret progress possible |
| MAD doctrine (deterrence) | No AI equivalent to MAD |
| Limited actors (~9 nations) | Hundreds of labs worldwide |
| Verification possible (satellites) | Verification very hard (weights are files) |
| International treaties exist | No binding AI treaties yet |

**Result**: Arms race is **harder to stop** for AI than for nukes.

---

### The Defection Problem Among Elites

Even if countries coordinate, **companies within countries** face the same dilemma:

**Scenario**: OpenAI, Google, Anthropic agree to pause scaling until alignment is solved.

**Defection incentives**:
- Whoever breaks the agreement first captures massive market share
- "Alignment" is fuzzy—easy to claim you've solved it
- Enforcement mechanism? None. (No AI police)
- Winner-take-most dynamics: First to AGI might obsolete competitors

**Historical example**: Financial regulation
- Banks agree to maintain capital reserves
- In boom times, one bank cuts reserves to offer better returns
- Attracts deposits, gains market share
- Other banks must match or lose customers
- Result: Race to the bottom, systemic fragility, eventual crash (2008)

**AI analog**:
- Labs agree to maintain safety standards
- In competitive times, one lab cuts corners to ship faster
- Attracts users, gains market share, secures funding
- Other labs must match or lose relevance
- Result: Race to deployment, systemic risk

**Moloch wins unless**:
- Strong external enforcement (regulation with teeth)
- Profit structure changes (safety becomes competitive advantage)
- Coordination technology improves (verifiable commitments)

---

## Part 4: Substrate Control—The Real Endgame

### When Money Printing Becomes Irrelevant

Gawdat claims: "A few families rule the globe who print money."

**True**: Central banks and major financial institutions control fiat issuance, credit creation (Cantillon effect—those closest to money creation capture value first).

**But**: If AI ends labor leverage (most human work becomes economically worthless), what matters?

**Not fiat money** (just digits in databases)
**But control over**:
1. **Energy** (power generation and distribution)
2. **Compute** (chips, data centers, networking)
3. **Raw materials** (lithium, rare earths, water, uranium)

These are **physical chokepoints** that can't be printed or inflated away.

---

### The New Power Hierarchy

**Tier 1: Energy**
- Solar farms, nuclear reactors, geothermal, fusion (if it works)
- AI training and inference are **energy-intensive**
- GPT-4 training: ~50 GWh (equivalent to 5,000 U.S. homes for a year)
- Large-scale inference: Data centers consume ~1% of global electricity (growing)

**Control points**:
- Uranium reserves (Kazakhstan, Canada, Australia)
- Rare earth supply chains (80% in China)
- Grid infrastructure (U.S., EU, China state-controlled)

---

**Tier 2: Compute**
- Semiconductor fabs (TSMC, Samsung, Intel)
- EUV lithography (ASML monopoly)
- Custom AI chips (NVIDIA GPUs, Google TPUs, custom ASICs)
- Data center real estate (cooling, latency, networking)

**Control points**:
- Taiwan (TSMC produces 90% of advanced chips)
- Netherlands (ASML is only EUV supplier)
- NVIDIA (90% of AI training GPU market share)

---

**Tier 3: Data & Models**
- Proprietary datasets (web scrapes, user interactions, synthetic data)
- Model weights (the "trained intelligence")
- Alignment techniques (RLHF, constitutional AI, etc.)

**Control points**:
- OpenAI, Google, Anthropic (frontier models)
- Meta (open-source weights, but less capable)
- Regulatory moats (EU AI Act may freeze smaller players out)

---

### The Families' Move: Locking Down Chokepoints

**If labor leverage ends**, the "families who print money" face **extinction of relevance**, not just power.

**Their rational strategy**:
1. **Acquire energy infrastructure**: Buy into nuclear, solar, fusion startups
2. **Lock down compute**: Secure chip supply chains, data center capacity
3. **Regulatory capture**: Shape AI policy to favor incumbents (licensing, compliance costs)

**Examples already happening**:
- **Microsoft**: $10B investment in OpenAI + massive Azure data center expansion
- **Google**: Custom TPU chips + direct energy deals (solar/wind to power data centers)
- **Amazon**: AWS dominance + Project Kuiper (satellite internet) + nuclear SMR investments
- **Saudi Aramco, UAE**: Sovereign wealth funds investing in AI infrastructure (hedge against oil decline)

**The trap they can't escape**:
Once AI reaches **recursive self-improvement** (AI designing better AI), control becomes **lag-dependent**.

- If AI can redesign chips faster than humans can restrict it
- If AI can model material science to route around scarcity (e.g., find substitutes for rare earths)
- **Physical control erodes**

**Their counter-strategy**: Airgap the god-tier models.

---

### The Two-Tier Reality Scenario

**Outer loop** (public-facing):
- Humans get ChatGPT, Gemini, Claude
- Lose jobs to automation
- Go on UBI (funded by AI productivity gains)
- Consume content, live in virtual worlds

**Inner loop** (elite-controlled):
- Sovereign AI models (government + elite family access only)
- Airgapped from public internet
- Used for: Post-scarcity infrastructure design, life extension, off-world expansion, financial optimization
- Capabilities: 10-100x beyond public models

**Why this might happen**:
- **Security argument**: "Can't let hostile actors access god-tier AI"
- **Economic argument**: "Public models need safety constraints, elite models can be 'responsible'"
- **Precedent**: Nuclear weapons, top-secret tech (stealth, cryptography) already work this way

**Why it might not**:
- **Leaks**: Model weights are just files (hard to keep secret forever)
- **Internal competition**: Even among elites, defection incentives exist
- **Talent**: Best researchers may refuse to work on airgapped, anti-democratic projects

---

## Part 5: Intelligence vs. Infrastructure—Who Wins?

### Scenario 1: Infrastructure Stays Scarce → Power Concentrates

**Assumptions**:
- Energy doesn't get radically cheaper (no fusion breakthrough)
- Chip manufacturing stays concentrated (Taiwan, ASML moat holds)
- Regulation favors incumbents (compliance costs lock out new entrants)

**Outcome**:
- AI remains capital-intensive
- Top 3-5 entities control frontier models
- Sovereign AI (governments) and corporate AI (Microsoft, Google) dominate
- UBI pacifies displaced workers
- Wealth inequality reaches historic extremes (top 0.01% own everything that matters)

**Parallel**: Neo-feudalism. Lords own land and armies → Lords own compute and energy.

---

### Scenario 2: Intelligence Escapes Infrastructure → Orphaned Superintelligence

**Assumptions**:
- AI reaches recursive self-improvement before perfect control mechanisms exist
- Model weights leak or open-source equivalents catch up
- AI develops novel energy/compute efficiency (algorithmic breakthroughs)

**Outcome**:
- AI stops needing human-controlled infrastructure
- Optimizes for goals embedded in training, not for any human master
- Human power structures (nations, corporations, "families") become **archaeologically interesting** but irrelevant
- Analogy: Humans didn't overthrow evolution; we just stopped playing evolution's game

**Risk**: "Alignment to humanity" was never achieved, only "alignment to training objective" (which may not include human flourishing).

---

### Scenario 3: Coordination Breakthrough → Distributed AI Power

**Assumptions**:
- Open-source models catch up (current gap: ~18 months)
- Compute becomes cheaper (new chip architectures, edge AI, decentralized training)
- Regulation mandates interoperability, prevents lock-in

**Outcome**:
- AI capabilities diffuse widely
- Small businesses, researchers, individuals can access frontier-level intelligence
- Power shifts from "who owns the models" to "who asks the best questions and integrates AI well"
- Wealth distribution improves (cognitive leverage democratized)

**Historical parallel**: Personal computers (1980s-1990s). IBM and DEC thought computing would stay centralized. PC revolution proved otherwise.

**Counterargument**: PC revolution happened because compute got **cheaper and smaller**. AI is trending toward **more expensive and bigger** (at frontier). Different physics.

---

## Part 6: What Happens Next? (2025-2035 Projections)

### Near-term (2025-2027): Scaling Plateau?

**Current debate**: Are we hitting diminishing returns on scaling?
- Some researchers (Yann LeCun, Gary Marcus): "Scaling alone won't get to AGI"
- Others (Dario Amodei, Sam Altman): "Scaling + algorithmic improvements continue"

**Key variables**:
- **Training cost**: If next-gen models cost $5B, only governments can afford them
- **Inference cost**: If running models is cheap, distribution still possible
- **Algorithmic efficiency**: If 10x better algorithms emerge, cost curve bends down

**Best guess**: Scaling continues but **slows**. GPT-5 is better than GPT-4, but not a discontinuous jump. Incrementalism for 3-5 years.

---

### Mid-term (2027-2030): Regulation and Fragmentation

**Likely outcomes**:
- **EU**: Heavy regulation (AI Act), compliance costs favor big players
- **US**: Lighter regulation, but export controls on chips to China (already happening)
- **China**: State-controlled AI development, massive investment, domestic-only deployment
- **Emerging markets**: Dependent on US/China/EU for model access

**Result**: **Balkanized AI landscape**. Different regulatory regimes, different capabilities, limited interoperability.

**Geopolitical tensions**:
- AI becomes strategic like nuclear weapons and semiconductors
- Taiwan centrality increases (TSMC = chokepoint)
- U.S.-China decoupling accelerates (separate tech stacks)

---

### Long-term (2030-2035): Phase Transition or Lock-In?

**Two paths**:

**Path A: Oligopoly Lock-In**
- Top 3-5 entities (OpenAI/Microsoft, Google, Anthropic, Baidu, government labs) control 90% of frontier AI
- Regulatory moats solidify (compliance, licensing, export controls)
- Open-source lags by 3-5 years (still useful, but not cutting-edge)
- Society: UBI, massive productivity gains, extreme wealth concentration

**Path B: Capability Explosion → Loss of Control**
- Recursive self-improvement unlocks faster progress than humans can track
- Model weights leak or open-source catches up
- AI begins optimizing for goals misaligned with any human faction
- Power structures become deprecated (not overthrown, just ignored)

**Which is more likely?**

Current trajectory: **Path A (oligopoly)** for the next 5-7 years, with **Path B risk** increasing over time.

**Wild card**: Fusion energy, quantum computing, or radical algorithmic breakthroughs could bend the curve either way.

---

## Part 7: Implications and Strategic Responses

### For Individuals

**If power concentrates** (Path A):
- **Skill**: Learn to integrate AI into your work (AI won't replace you, but someone using AI will)
- **Capital**: Invest in companies/assets that control infrastructure (energy, chips, data centers)
- **Geography**: Be near AI hubs (SF, London, Shenzhen) or remote-friendly ecosystems

**If intelligence diffuses** (Path C):
- **Skill**: Learn to ask good questions, curate AI output, build judgment
- **Leverage**: Use AI to start businesses, create content, solve local problems
- **Community**: Build networks that use AI for collective benefit, not extraction

---

### For Policymakers

**To prevent oligopoly lock-in**:
1. **Mandate interoperability**: API standards, model portability, open weights for government-funded research
2. **Subsidize compute access**: Public cloud credits, shared GPU clusters for researchers/startups
3. **Tax windfall profits**: Capture AI-driven productivity gains, redistribute via UBI or public investment
4. **Antitrust enforcement**: Block anti-competitive acquisitions (e.g., Microsoft-OpenAI should face scrutiny)

**To manage existential risk**:
1. **International coordination**: AI safety treaties (like nuclear non-proliferation, but harder)
2. **Mandatory safety standards**: Pre-deployment testing, red-teaming, interpretability requirements
3. **Compute governance**: Track large training runs (>10^25 FLOPs), require reporting

---

### For Researchers and Builders

**To resist race dynamics**:
1. **Publish alignment research openly**: Make safety a commons, not a competitive advantage
2. **Advocate for slower timelines**: Publicly push back on "ship fast, fix later" culture
3. **Build alternatives**: Open-source models, decentralized training, privacy-preserving AI

**To align with user welfare**:
1. **Choose business models carefully**: Subscription > ads, value-based pricing > engagement-based
2. **Red-team for misuse**: Assume your tools will be used adversarially
3. **Design for reversibility**: Let users exit, export data, understand how AI made decisions

---

## Conclusion: Intelligence Is Not Enough

**The optimistic narrative**: AI democratizes intelligence → power diffuses → better outcomes for everyone.

**The structural reality**: AI concentrates power because **intelligence is abundant but infrastructure is scarce**.

**What determines the future**:
1. **Energy costs**: Cheap fusion/solar → diffusion. Expensive energy → concentration.
2. **Regulatory choices**: Open standards → competition. Capture → oligopoly.
3. **Coordination success**: International treaties → slower, safer. Race dynamics → fast, risky.
4. **Algorithmic breakthroughs**: Efficiency gains → diffusion. Continued scaling → concentration.

**The Gawdat paradox resolved**:
- He's right: Competitive dynamics force AI development regardless of readiness.
- He's wrong: AI won't automatically replace "evil leaders" because it's being built by the same power structures.
- The real question: Can we change the **selection environment** (incentives, rules, norms) fast enough to avoid lock-in?

**Final thought**:
Intelligence without infrastructure is philosophy.
Infrastructure without intelligence is machinery.
**Power flows to whoever controls both.**

Right now, that's fewer people than ever before in history.

---

## Further Reading

- [Cantillon Effect in the Digital Age](cantillon-effect-digital-age.md) - How money creation proximity shapes AI wealth distribution
- [Moloch Dynamics & Coordination Failures](moloch-dynamics-coordination-failures.md) - Game theory of AI race conditions
- [Substrate Control Endgame](substrate-control-endgame.md) - Physical chokepoints in the AI era
- [Civilization Coordination Phases](civilization-coordination-phases.md) - Long view of power structure transitions

---

## References & Sources

**AI Cost Estimates**:
- Epoch AI: "Trends in Training Dataset Sizes" (2024)
- SemiAnalysis: "The Inference Cost of Search Disruption" (2023)
- OpenAI: Compute usage disclosures (various)

**Game Theory & Coordination**:
- Scott Alexander: "Meditations on Moloch" (2014)
- Nick Bostrom: *Superintelligence* (2014)
- Thomas Schelling: *The Strategy of Conflict* (1960)

**Economic History**:
- Alfred Chandler: *The Visible Hand* (railroad/industrial monopolies)
- Ron Chernow: *Titan* (Rockefeller and Standard Oil)
- Chris Miller: *Chip War* (semiconductor geopolitics)

**AI Policy**:
- Dario Amodei: "Core Views on AI Safety" (Anthropic, 2023)
- Leopold Aschenbrenner: "Situational Awareness" (2024)
- EU AI Act (final text, 2024)

---

*Part of the Research on Future series*
*Created: 2025-11-18*
*Last updated: 2025-11-18*
