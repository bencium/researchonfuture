# Goodhart's Law in Product Design
## When Metrics Become Targets, Value Gets Destroyed

*"When a measure becomes a target, it ceases to be a good measure."* — Charles Goodhart (1975)

---

## The Core Problem

Every product team wants to move fast and measure progress. So you pick metrics:
- **Engagement time** (how long users stay)
- **Conversion rate** (how many sign up / pay)
- **Daily active users** (DAU)
- **Click-through rate** (CTR)

Then you optimize. Run A/B tests. Ship the variant that wins. Repeat.

**The trap**: These metrics are *proxies* for value. But once you optimize for the proxy, you destroy the thing it was measuring.

---

## How It Happens: A Worked Example

**Goal**: Build a product people love
**Proxy metric**: Engagement time (session duration)
**Logic**: "If people spend more time, they must love it"

**What you test**:
- Variant A: Clean interface, fast, gets users to their goal
- Variant B: Adds friction, "related content" rabbit holes, popups

**Result**: Variant B wins. Session duration +18%.

**What you ship**: Variant B

**What actually happened**: You didn't increase love. You increased **friction and distraction**. Users spend more time because it's harder to leave, not because it's more valuable.

After 6 months:
- Churn increases (people realize they're wasting time)
- Trust declines (feels manipulative)
- Brand perception shifts (from "useful tool" to "time sink")

**Goodhart in action**: The metric (session time) no longer correlates with the goal (love) because you optimized for the metric directly.

---

## The Mechanism: Why Optimization Corrupts Proxies

1. **Proxies are imperfect**
   They correlate with the goal *in the natural state*, but the correlation is fragile.

2. **Optimization amplifies edge cases**
   A/B testing finds interventions that move the metric. These are often exploits, not improvements.

3. **Unmeasured values get cannibalized**
   You optimize measured dimensions (clicks, time) at the expense of unmeasured ones (trust, dignity, clarity).

4. **Feedback loops are slow**
   Metric wins are immediate. Trust erosion shows up months later. By then, the team is 10 experiments downstream.

---

## Real-World Product Examples

### Facebook News Feed (2010s)
**Goal**: Connect people, share meaningful content
**Metric**: Engagement (likes, comments, shares, time-spent)
**Optimization**: Prioritize content that triggers emotional reactions
**Result**: Outrage and polarization spread faster than nuance. "Meaningful connections" became "arguments with strangers."
**Outcome**: Metric hit all-time highs while trust and user satisfaction declined.

---

### YouTube Recommendations (2015-2020)
**Goal**: Help people discover great videos
**Metric**: Watch time (total minutes watched)
**Optimization**: Recommend videos that maximize binge-watching
**Result**: Algorithm promotes conspiracy theories, extreme content, auto-play rabbit holes
**Outcome**: Watch time skyrocketed. Radicalization and misinformation also skyrocketed.

---

### E-commerce Conversion Funnels
**Goal**: Help customers find what they need
**Metric**: Conversion rate (purchases / visitors)
**Optimization**: Dark patterns (fake scarcity, pre-checked boxes, confusing opt-outs)
**Result**: Short-term conversion lift +12%. Long-term trust penalty, higher returns, customer service costs.
**Outcome**: Optimized for first purchase, destroyed repeat customer value.

---

### Mobile Game Retention
**Goal**: Create fun, engaging games
**Metric**: DAU, session frequency
**Optimization**: Streaks, daily rewards, FOMO mechanics, energy systems
**Result**: Players feel obligated to log in, not excited
**Outcome**: High DAU, low genuine enjoyment. Players eventually burn out and leave bitter.

---

## The Business Model Dependency

**Why it's hard to escape**:
- Your business model determines which metrics you *must* hit to survive
- Ad-driven products *need* engagement time → manipulative features are "rational"
- Freemium products *need* conversion pressure → dark patterns at paywalls are "necessary"

**Examples**:

| Business Model | Core Metric | Goodhart Risk | Typical Pattern |
|----------------|-------------|---------------|-----------------|
| **Advertising** | Time spent, impressions | High | Infinite scroll, clickbait, outrage amplification |
| **Freemium** | Conversion rate | High | Artificial feature limits, confusing pricing, fake urgency |
| **Subscription** | Retention, churn | Medium | Friction to cancel, auto-renewal tricks, guilt messaging |
| **Transaction fee** | Volume | Medium | Hidden fees, complex pricing, upselling |
| **Enterprise SaaS** | Net retention, expansion | Low | Long sales cycles reward actual value delivery |

**Key insight**: Some business models align better with user welfare than others. If your model requires Goodhart-exploited metrics to survive, your product will degrade over time.

---

## How to Fight Goodhart's Law

### 1. Use Multi-Metric Scorecards (with penalties)

Don't optimize a single metric. Create a **North Star with constraints**.

**Example**:
```
Product Health Score =
  (Revenue Growth × 0.4) +
  (User Satisfaction × 0.3) +
  (Retention × 0.3) -
  (Trust Penalties × 2.0)

Trust Penalties:
- Customer service complaints per user
- Cancellation friction (clicks to cancel)
- Feature obfuscation score (UX review)
- Regret actions (undo, unsubscribe within 24h)
```

The **penalty multiplier** (×2.0) ensures you can't offset trust damage with revenue gains.

---

### 2. Measure What You Actually Care About

**Bad proxies** (Goodhart-vulnerable):
- Session duration → Could be friction, not value
- Click-through rate → Could be clickbait
- Sign-ups → Could be dark patterns

**Better proxies** (harder to game):
- **Net Promoter Score (NPS)** → Would you recommend this?
- **Repeat usage without prompts** → Did they come back organically?
- **Task success rate** → Did they accomplish their goal?
- **Time to value** → How fast did they get utility?

**Gold standard** (very hard to game):
- **Customer lifetime value (LTV)** → Long-term revenue from happy customers
- **Referral rate** → Do users bring friends?
- **Survivorship without nags** → Retention without push notifications / emails

---

### 3. Red-Team Your Metrics

Before committing to a metric, ask:
- **How would I game this metric without providing value?**
- **What's the sleaziest way to move this number?**
- **If we hit this metric but users hate us, what happened?**

Run this exercise quarterly. If your team can easily list 5 ways to game your core metrics, **you will game them** (even unintentionally, via A/B testing).

---

### 4. Encode Reversibility and Consent

Make **user agency** a first-class feature:
- One-click cancel (no "are you sure?" guilt)
- Data export (full portability)
- Undo/regret actions (easy reversion)
- Consent freshness (re-confirm annually)

**Track these**:
- Time-to-cancel (in clicks and seconds)
- Data export usage (how many users exercise this?)
- Undo rate (what % of actions get reversed?)

If these metrics get worse over time, you're drifting toward manipulation.

---

### 5. Choose Business Models That Align With User Welfare

**High alignment**:
- **Subscription (for ongoing value)**: Revenue tied to retention → must keep delivering
- **Transaction fees (on user success)**: Only make money when users win (Stripe, Shopify)
- **Freemium (generous free tier)**: Free tier is useful, paid tier is 10x better (not crippled free)

**Low alignment**:
- **Advertising (attention-based)**: Revenue tied to time-spent → incentive to waste time
- **Freemium (crippled free tier)**: Free tier is frustrating → dark patterns to convert
- **One-time purchase (no updates)**: Incentive to ship and abandon

**Strategic choice**: If you pick an ads model, you *will* fight Goodhart battles forever. If you pick subscription-with-generous-trial, your incentives naturally align with user satisfaction.

---

## Case Study: Basecamp vs. Asana

**Basecamp**:
- Business model: Flat-rate subscription ($99/month, unlimited users)
- Core metric: Customer satisfaction, retention
- Product philosophy: Calm, simple, no notifications spam, no growth hacks
- Result: Slower growth, but near-zero churn, rabid fans, 20+ year sustainability

**Asana** (early years):
- Business model: Freemium, per-seat pricing
- Core metric: User activation, paid conversion
- Product philosophy: Feature-rich, integrations, onboarding flows
- Result: Faster growth, higher churn, more complexity, eventual pivot to enterprise focus

**Neither is "wrong"**, but Basecamp's model made Goodhart-resistance easier. Asana had to work harder to avoid dark patterns because conversion pressure was central to survival.

---

## Takeaways for Builders

1. **All metrics are proxies.** The moment you optimize them, they decouple from the goal.

2. **Your business model predetermines your ethical constraints.** Choose wisely at founding.

3. **Use multi-metric scorecards with penalties.** Don't let revenue wins offset trust damage.

4. **Red-team your metrics quarterly.** If you can game them, your A/B tests will.

5. **Measure user agency.** Time-to-cancel, data export, undo rates are anti-Goodhart signals.

6. **Long-term scorecards beat short-term wins.** Optimize for LTV, referrals, and retention-without-nags, not session duration.

---

**Further reading**:
- [Dark Patterns & Systemic Misalignment](dark-patterns-systemic-misalignment.md) - Why markets select for manipulation
- [Business Model Ethical Constraints](business-model-ethical-constraints.md) - Revenue model determines boundaries
- [Systems Thinking Primer](systems-thinking-primer.md) - Feedback loops and emergent dysfunction

---

## References & Deep Dives

- **Charles Goodhart** (1975): Original formulation in monetary policy
- **Marilyn Strathern** (1997): "'When a measure becomes a target, it ceases to be a good measure' applies beyond economics"
- **Jerry Muller** (2018): *The Tyranny of Metrics* - How measurement distorts what it measures
- **Campbell's Law** (1976): "The more any quantitative social indicator is used for decision-making, the more subject it will be to corruption pressures"

---

*Part of the Research on Future series*
*Created: 2025-11-18*
