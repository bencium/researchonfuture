# CLAUDE.md - AI Assistant Guide

## Repository Overview

**researchonfuture** is a research repository focused on deep analytical exploration of societal systems, economic structures, and civilizational patterns. The content examines fundamental questions about power, institutions, technology, and human coordination through a systems-thinking lens.

### Purpose

This repository serves as a collection of analytical essays and dialogues exploring:
- Economic systems and capitalism's structural dynamics
- AI development and its relationship to power structures
- Historical patterns in human civilization and leadership
- Institutional design and incentive structures
- Market dynamics, software/UX, and user behavior
- Future scenarios and phase transitions in human society

### Target Audience

- Researchers and thinkers interested in systems analysis
- Those studying economic and political structures
- People exploring AI's impact on society and power dynamics
- Anyone interested in deep, critical thinking about civilization

## Repository Structure

```
researchonfuture/
├── CLAUDE.md           # This file - AI assistant guide
├── capitalism.md       # Analysis of capitalism, AI, and power structures
└── human-history.md    # Exploration of historical patterns and civilizational dynamics
```

### Core Files

#### `capitalism.md`
**Focus**: Critical analysis of capitalism, power concentration, and AI's role in economic systems

**Key themes**:
- Mo Gawdat's views on capitalism and AI
- Prisoner's dilemma dynamics in AI development
- Cantillonaire theory and money creation
- Capital concentration and AI infrastructure
- Future scenarios: UBI, feudalism, AI autonomy
- Power structures and substrate control
- Alignment races between elite factions

**Content style**: Analytical, philosophical, focuses on incentive structures and power dynamics

#### `human-history.md`
**Focus**: Long-arc historical analysis of human civilization and institutions

**Key themes**:
- Historical patterns across millennia (10,000+ years)
- Energy, information, and coordination as civilizational drivers
- Era classification (Internet, Platform/Feed, Crisis/Acceleration)
- Leadership selection mechanisms across history
- "Micro-dwarfs" concept (expressive power vs structural power)
- Institutional design and its persistent flaws
- Software/UX as encoded value systems
- Market selection dynamics for companies and products

**Content style**: Conversational dialogue format, systems analysis, historical pattern recognition

## Development Workflows

### Adding New Content

1. **Research Files**: Create new markdown files following the pattern:
   - Use lowercase with hyphens for filenames (e.g., `future-scenarios.md`)
   - Focus on analytical depth over breadth
   - Use clear section headers with `##` and `###`
   - Include philosophical/critical perspective

2. **Content Structure**:
   - Start with clear framing of the question or topic
   - Use numbered or bulleted lists for clarity
   - Include subsections with descriptive headers
   - Use block quotes `>` for key definitions or concepts
   - Use horizontal rules `---` to separate major sections

3. **Writing Style**:
   - Analytical and systems-oriented
   - Avoid emotional language; focus on mechanisms and incentives
   - Use concrete examples and historical patterns
   - Define terms explicitly when introducing new concepts
   - Conversational tone is acceptable for dialogue-style content

### Git Workflow

This repository follows a standard git workflow:

```bash
# Check status
git status

# Add new or modified files
git add <filename>

# Commit with descriptive message
git commit -m "Add analysis of [topic]"

# Push to current branch
git push -u origin <branch-name>
```

**Branch naming**: Feature branches should start with `claude/` prefix followed by descriptive identifier

**Commit messages**: Should be clear and descriptive:
- ✅ "Add analysis of institutional design failures"
- ✅ "Expand capitalism.md with AI alignment race discussion"
- ❌ "Update file"
- ❌ "Changes"

## Key Conventions for AI Assistants

### Content Philosophy

1. **Systems Thinking**: Always analyze topics through the lens of:
   - Incentive structures
   - Selection mechanisms
   - Feedback loops
   - Power dynamics
   - Coordination problems

2. **Historical Calibration**: Ground analysis in historical patterns rather than recent noise. Ask:
   - Is this genuinely new, or familiar dynamics in new clothing?
   - What are the relevant timescales (decades, centuries, millennia)?
   - What selection pressures shaped current structures?

3. **Avoid Moralizing**: Focus on mechanisms over judgments:
   - ✅ "This incentive structure selects for X behavior"
   - ❌ "People are bad because they do X"
   - Describe what optimizes for what, not what "should" happen

4. **Precision Over Performance**:
   - Define terms explicitly
   - Separate correlation from causation
   - Acknowledge uncertainty
   - Distinguish descriptive from normative claims

### Writing Guidelines

1. **Structure**:
   - Use numbered sections for sequential logic
   - Use bullets for lists of related items
   - Use horizontal rules to separate distinct topics
   - Keep paragraphs focused (3-5 sentences typically)

2. **Terminology**:
   - Introduce new concepts with clear definitions
   - Use block quotes for key definitions
   - Maintain consistency in terminology
   - Avoid jargon unless necessary (then define it)

3. **Analysis Depth**:
   - Go beyond surface observations
   - Identify second and third-order effects
   - Connect to broader patterns
   - Consider multiple timescales
   - Map out game-theoretic dynamics

4. **Examples and Evidence**:
   - Use historical examples when available
   - Reference specific mechanisms (e.g., "A/B testing selects for...")
   - Distinguish between "seems like" and "demonstrably is"
   - Acknowledge where you're reasoning by analogy

### Common Patterns to Follow

#### The "Zoom Out" Pattern
```markdown
## [Question or Topic]

Short answer: [1-2 sentence direct answer]

Let me zoom out and then zoom in.

---

## 1. [Broader Context]
[Historical or structural framing]

## 2. [Specific Analysis]
[Detailed examination]

## 3. [Implications]
[What this means going forward]
```

#### The "Lens Comparison" Pattern
```markdown
Three lenses:

1. **[First Lens Name]**
   * [Observation from this angle]
   * [Key insight]

2. **[Second Lens Name]**
   * [Different observation]
   * [Different insight]

3. **[Third Lens Name]**
   * [Yet another perspective]
   * [Synthesis]
```

#### The "Normal vs Different" Pattern
```markdown
### Things that *are* "normal cycle"
- [Pattern that repeats historically]
- [Another recurring pattern]

### Things that are genuinely different in kind
- [Novel dynamic]
- [Unprecedented element]
```

### Questions to Ask When Adding Content

Before adding new content, consider:

1. **Scope**: What historical timeframe is relevant? (Years? Decades? Millennia?)
2. **Mechanisms**: What selection pressures or incentive structures drive the pattern?
3. **Novelty**: Is this actually new, or old dynamics with new aesthetics?
4. **Leverage**: Where can individual or small-group action actually change outcomes?
5. **Timescales**: What feedback loops operate over what timeframes?

### Anti-Patterns to Avoid

1. ❌ **Recency Bias**: Treating the last 5-10 years as uniquely unprecedented without historical grounding
2. ❌ **Moral Framing**: "X is bad" instead of "X optimizes for Y, which creates Z outcomes"
3. ❌ **Solutionism**: Jumping to "how to fix it" before fully understanding the system
4. ❌ **False Precision**: Claiming certainty where there's uncertainty
5. ❌ **Narrative Compression**: Reducing complex dynamics to simple stories
6. ❌ **Clickbait Language**: Using emotional or exaggerated terms instead of precise description

## Technical Considerations

### File Format
- All content files are Markdown (`.md`)
- Use UTF-8 encoding
- Line length is not strictly enforced but aim for readability
- Use `→` character for continuation or emphasis where appropriate

### Markdown Style
- Headers: `#` for title, `##` for major sections, `###` for subsections
- Lists: Use `*` or `-` for bullets, numbers for sequential items
- Emphasis: `**bold**` for key terms, `*italic*` for emphasis
- Code/technical terms: Use backticks when referencing `technical concepts`
- Block quotes: Use `>` for definitions or key quotations
- Horizontal rules: `---` to separate major sections

### Version Control
- Commit atomically (one logical change per commit)
- Write clear commit messages explaining *what* and *why*
- Keep the working directory clean
- Don't commit temporary or generated files

## Collaboration Guidelines

### When Adding New Analysis

1. **Read Existing Content**: Understand the tone, depth, and style already established
2. **Identify Connections**: Link new content to existing themes where relevant
3. **Maintain Consistency**: Use similar analytical frameworks and terminology
4. **Avoid Redundancy**: Build on existing analysis rather than repeating it
5. **Cross-Reference**: Mention related sections in other files when applicable

### When Updating Existing Content

1. **Preserve Intent**: Maintain the original analytical direction
2. **Extend, Don't Replace**: Add depth rather than rewriting unless clearly wrong
3. **Mark Major Changes**: In commit messages, note if significantly altering existing analysis
4. **Maintain Voice**: Keep the established conversational/analytical tone

## Future Directions

Potential areas for expansion (not prescriptive, just observed gaps):

- **Technology & Society**: Deep dives into specific technologies (blockchain, biotech, etc.)
- **Coordination Mechanisms**: Analysis of new governance and coordination tools
- **Alternative Systems**: Exploration of non-capitalist economic models
- **AI Alignment**: Technical and social aspects of AI development paths
- **Institutional Innovation**: Concrete examples of better-designed institutions
- **Local Forks**: Practical guides for building "non-deranged" local systems

## Meta-Notes for AI Assistants

### When Working with This Repository

1. **Understand the Mission**: This is analytical research, not advocacy or documentation
2. **Match the Depth**: Responses should be thoughtful, not quick takes
3. **Use the Patterns**: Follow established structural and analytical patterns
4. **Think Systems**: Always analyze through incentives, selection, and feedback loops
5. **Ground Historically**: Reference patterns across long timescales
6. **Be Precise**: Define terms, acknowledge uncertainty, separate is from ought

### Optimization Targets

When writing for this repository, optimize for:
- **Clarity of mechanism**: Can the reader understand *how* something works?
- **Historical grounding**: Is this calibrated against long-arc patterns?
- **Actionable insight**: Does this help readers think more clearly?
- **Intellectual honesty**: Are uncertainties and limitations acknowledged?

Do NOT optimize for:
- Engagement or virality
- Confirming existing beliefs
- Emotional resonance over accuracy
- Simplified narratives that obscure complexity

## Quick Reference

### Common Concepts in This Repository

- **Selection pressures**: Forces that determine which behaviors/systems survive
- **Incentive structures**: What actions are rewarded or punished in a system
- **Feedback loops**: How outputs influence inputs over time
- **Goodhart's Law**: When a measure becomes a target, it ceases to be a good measure
- **Moloch dynamics**: Coordination failures where individual rationality leads to collective disaster
- **Substrate control**: Power through controlling fundamental infrastructure
- **Micro-dwarfs**: People with high expressive power but low structural power
- **Phase transition**: Fundamental shifts in how systems operate

### Questions This Repository Explores

- How do power structures select for certain types of leaders?
- What happens when AI becomes the dominant force in economic systems?
- How do markets select for software and companies?
- What patterns repeat across civilizational transitions?
- How do institutions fail, and can they be designed better?
- What's genuinely new vs. old patterns in new clothing?

---

**Last Updated**: 2025-11-18

**Repository Maintainer**: Research on Future Analysis Project

**For AI Assistants**: This is a living document. Update it as patterns emerge or the repository evolves. Always maintain analytical rigor and intellectual honesty.
