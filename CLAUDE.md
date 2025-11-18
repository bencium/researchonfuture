# Claude Code Configuration - SPARC Development Environment

## 🚨 CRITICAL: CONCURRENT EXECUTION & FILE MANAGEMENT

**ABSOLUTE RULES**:
1. ALL operations MUST be concurrent/parallel in a single message
2. **NEVER save working files, text/mds and tests to the root folder**
3. ALWAYS organize files in appropriate subdirectories
4. **USE CLAUDE CODE'S TASK TOOL** for spawning agents concurrently, not just MCP

### ⚡ GOLDEN RULE: "1 MESSAGE = ALL RELATED OPERATIONS"

**MANDATORY PATTERNS:**
- **TodoWrite**: ALWAYS batch ALL todos in ONE call (5-10+ todos minimum)
- **Task tool (Claude Code)**: ALWAYS spawn ALL agents in ONE message with full instructions
- **File operations**: ALWAYS batch ALL reads/writes/edits in ONE message
- **Bash commands**: ALWAYS batch ALL terminal operations in ONE message
- **Memory operations**: ALWAYS batch ALL memory store/retrieve in ONE message

### 🎯 CRITICAL: Claude Code Task Tool for Agent Execution

**Claude Code's Task tool is the PRIMARY way to spawn agents:**
```javascript
// ✅ CORRECT: Use Claude Code's Task tool for parallel agent execution
[Single Message]:
  Task("Research agent", "Analyze requirements and patterns...", "researcher")
  Task("Coder agent", "Implement core features...", "coder")
  Task("Tester agent", "Create comprehensive tests...", "tester")
  Task("Reviewer agent", "Review code quality...", "reviewer")
  Task("Architect agent", "Design system architecture...", "system-architect")
```

**MCP tools are ONLY for coordination setup:**
- `mcp__claude-flow__swarm_init` - Initialize coordination topology
- `mcp__claude-flow__agent_spawn` - Define agent types for coordination
- `mcp__claude-flow__task_orchestrate` - Orchestrate high-level workflows

### 📁 File Organization Rules

**NEVER save to root folder. Use these directories:**
- `/src` - Source code files
- `/tests` - Test files
- `/docs` - Documentation and markdown files
- `/config` - Configuration files
- `/scripts` - Utility scripts
- `/examples` - Example code

## Project Overview

This project uses SPARC (Specification, Pseudocode, Architecture, Refinement, Completion) methodology with Claude-Flow orchestration for systematic Test-Driven Development.

## SPARC Commands

### Core Commands
- `npx claude-flow sparc modes` - List available modes
- `npx claude-flow sparc run <mode> "<task>"` - Execute specific mode
- `npx claude-flow sparc tdd "<feature>"` - Run complete TDD workflow
- `npx claude-flow sparc info <mode>` - Get mode details

### Batchtools Commands
- `npx claude-flow sparc batch <modes> "<task>"` - Parallel execution
- `npx claude-flow sparc pipeline "<task>"` - Full pipeline processing
- `npx claude-flow sparc concurrent <mode> "<tasks-file>"` - Multi-task processing

### Build Commands
- `npm run build` - Build project
- `npm run test` - Run tests
- `npm run lint` - Linting
- `npm run typecheck` - Type checking

## SPARC Workflow Phases

1. **Specification** - Requirements analysis (`sparc run spec-pseudocode`)
2. **Pseudocode** - Algorithm design (`sparc run spec-pseudocode`)
3. **Architecture** - System design (`sparc run architect`)
4. **Refinement** - TDD implementation (`sparc tdd`)
5. **Completion** - Integration (`sparc run integration`)

## Code Style & Best Practices

- **Modular Design**: Files under 500 lines
- **Environment Safety**: Never hardcode secrets
- **Test-First**: Write tests before implementation
- **Clean Architecture**: Separate concerns
- **Documentation**: Keep updated

## 🚀 Available Agents (54 Total)

### Core Development
`coder`, `reviewer`, `tester`, `planner`, `researcher`

### Swarm Coordination
`hierarchical-coordinator`, `mesh-coordinator`, `adaptive-coordinator`, `collective-intelligence-coordinator`, `swarm-memory-manager`

### Consensus & Distributed
`byzantine-coordinator`, `raft-manager`, `gossip-coordinator`, `consensus-builder`, `crdt-synchronizer`, `quorum-manager`, `security-manager`

### Performance & Optimization
`perf-analyzer`, `performance-benchmarker`, `task-orchestrator`, `memory-coordinator`, `smart-agent`

### GitHub & Repository
`github-modes`, `pr-manager`, `code-review-swarm`, `issue-tracker`, `release-manager`, `workflow-automation`, `project-board-sync`, `repo-architect`, `multi-repo-swarm`

### SPARC Methodology
`sparc-coord`, `sparc-coder`, `specification`, `pseudocode`, `architecture`, `refinement`

### Specialized Development
`backend-dev`, `mobile-dev`, `ml-developer`, `cicd-engineer`, `api-docs`, `system-architect`, `code-analyzer`, `base-template-generator`

### Testing & Validation
`tdd-london-swarm`, `production-validator`

### Migration & Planning
`migration-planner`, `swarm-init`

## 🎯 Claude Code vs MCP Tools

### Claude Code Handles ALL EXECUTION:
- **Task tool**: Spawn and run agents concurrently for actual work
- File operations (Read, Write, Edit, MultiEdit, Glob, Grep)
- Code generation and programming
- Bash commands and system operations
- Implementation work
- Project navigation and analysis
- TodoWrite and task management
- Git operations
- Package management
- Testing and debugging

### MCP Tools ONLY COORDINATE:
- Swarm initialization (topology setup)
- Agent type definitions (coordination patterns)
- Task orchestration (high-level planning)
- Memory management
- Neural features
- Performance tracking
- GitHub integration

**KEY**: MCP coordinates the strategy, Claude Code's Task tool executes with real agents.

## 🚀 Quick Setup

```bash
# Add MCP servers (Claude Flow required, others optional)
claude mcp add claude-flow npx claude-flow@alpha mcp start
claude mcp add ruv-swarm npx ruv-swarm mcp start  # Optional: Enhanced coordination
claude mcp add flow-nexus npx flow-nexus@latest mcp start  # Optional: Cloud features
```

## MCP Tool Categories

### Coordination
`swarm_init`, `agent_spawn`, `task_orchestrate`

### Monitoring
`swarm_status`, `agent_list`, `agent_metrics`, `task_status`, `task_results`

### Memory & Neural
`memory_usage`, `neural_status`, `neural_train`, `neural_patterns`

### GitHub Integration
`github_swarm`, `repo_analyze`, `pr_enhance`, `issue_triage`, `code_review`

### System
`benchmark_run`, `features_detect`, `swarm_monitor`

### Flow-Nexus MCP Tools (Optional Advanced Features)
Flow-Nexus extends MCP capabilities with 70+ cloud-based orchestration tools:

**Key MCP Tool Categories:**
- **Swarm & Agents**: `swarm_init`, `swarm_scale`, `agent_spawn`, `task_orchestrate`
- **Sandboxes**: `sandbox_create`, `sandbox_execute`, `sandbox_upload` (cloud execution)
- **Templates**: `template_list`, `template_deploy` (pre-built project templates)
- **Neural AI**: `neural_train`, `neural_patterns`, `seraphina_chat` (AI assistant)
- **GitHub**: `github_repo_analyze`, `github_pr_manage` (repository management)
- **Real-time**: `execution_stream_subscribe`, `realtime_subscribe` (live monitoring)
- **Storage**: `storage_upload`, `storage_list` (cloud file management)

**Authentication Required:**
- Register: `mcp__flow-nexus__user_register` or `npx flow-nexus@latest register`
- Login: `mcp__flow-nexus__user_login` or `npx flow-nexus@latest login`
- Access 70+ specialized MCP tools for advanced orchestration

## 🚀 Agent Execution Flow with Claude Code

### The Correct Pattern:

1. **Optional**: Use MCP tools to set up coordination topology
2. **REQUIRED**: Use Claude Code's Task tool to spawn agents that do actual work
3. **REQUIRED**: Each agent runs hooks for coordination
4. **REQUIRED**: Batch all operations in single messages

### Example Full-Stack Development:

```javascript
// Single message with all agent spawning via Claude Code's Task tool
[Parallel Agent Execution]:
  Task("Backend Developer", "Build REST API with Express. Use hooks for coordination.", "backend-dev")
  Task("Frontend Developer", "Create React UI. Coordinate with backend via memory.", "coder")
  Task("Database Architect", "Design PostgreSQL schema. Store schema in memory.", "code-analyzer")
  Task("Test Engineer", "Write Jest tests. Check memory for API contracts.", "tester")
  Task("DevOps Engineer", "Setup Docker and CI/CD. Document in memory.", "cicd-engineer")
  Task("Security Auditor", "Review authentication. Report findings via hooks.", "reviewer")
  
  // All todos batched together
  TodoWrite { todos: [...8-10 todos...] }
  
  // All file operations together
  Write "backend/server.js"
  Write "frontend/App.jsx"
  Write "database/schema.sql"
```

## 📋 Agent Coordination Protocol

### Every Agent Spawned via Task Tool MUST:

**1️⃣ BEFORE Work:**
```bash
npx claude-flow@alpha hooks pre-task --description "[task]"
npx claude-flow@alpha hooks session-restore --session-id "swarm-[id]"
```

**2️⃣ DURING Work:**
```bash
npx claude-flow@alpha hooks post-edit --file "[file]" --memory-key "swarm/[agent]/[step]"
npx claude-flow@alpha hooks notify --message "[what was done]"
```

**3️⃣ AFTER Work:**
```bash
npx claude-flow@alpha hooks post-task --task-id "[task]"
npx claude-flow@alpha hooks session-end --export-metrics true
```

## 🎯 Concurrent Execution Examples

### ✅ CORRECT WORKFLOW: MCP Coordinates, Claude Code Executes

```javascript
// Step 1: MCP tools set up coordination (optional, for complex tasks)
[Single Message - Coordination Setup]:
  mcp__claude-flow__swarm_init { topology: "mesh", maxAgents: 6 }
  mcp__claude-flow__agent_spawn { type: "researcher" }
  mcp__claude-flow__agent_spawn { type: "coder" }
  mcp__claude-flow__agent_spawn { type: "tester" }

// Step 2: Claude Code Task tool spawns ACTUAL agents that do the work
[Single Message - Parallel Agent Execution]:
  // Claude Code's Task tool spawns real agents concurrently
  Task("Research agent", "Analyze API requirements and best practices. Check memory for prior decisions.", "researcher")
  Task("Coder agent", "Implement REST endpoints with authentication. Coordinate via hooks.", "coder")
  Task("Database agent", "Design and implement database schema. Store decisions in memory.", "code-analyzer")
  Task("Tester agent", "Create comprehensive test suite with 90% coverage.", "tester")
  Task("Reviewer agent", "Review code quality and security. Document findings.", "reviewer")
  
  // Batch ALL todos in ONE call
  TodoWrite { todos: [
    {id: "1", content: "Research API patterns", status: "in_progress", priority: "high"},
    {id: "2", content: "Design database schema", status: "in_progress", priority: "high"},
    {id: "3", content: "Implement authentication", status: "pending", priority: "high"},
    {id: "4", content: "Build REST endpoints", status: "pending", priority: "high"},
    {id: "5", content: "Write unit tests", status: "pending", priority: "medium"},
    {id: "6", content: "Integration tests", status: "pending", priority: "medium"},
    {id: "7", content: "API documentation", status: "pending", priority: "low"},
    {id: "8", content: "Performance optimization", status: "pending", priority: "low"}
  ]}
  
  // Parallel file operations
  Bash "mkdir -p app/{src,tests,docs,config}"
  Write "app/package.json"
  Write "app/src/server.js"
  Write "app/tests/server.test.js"
  Write "app/docs/API.md"
```

### ❌ WRONG (Multiple Messages):
```javascript
Message 1: mcp__claude-flow__swarm_init
Message 2: Task("agent 1")
Message 3: TodoWrite { todos: [single todo] }
Message 4: Write "file.js"
// This breaks parallel coordination!
```

## Performance Benefits

- **84.8% SWE-Bench solve rate**
- **32.3% token reduction**
- **2.8-4.4x speed improvement**
- **27+ neural models**

## Hooks Integration

### Pre-Operation
- Auto-assign agents by file type
- Validate commands for safety
- Prepare resources automatically
- Optimize topology by complexity
- Cache searches

### Post-Operation
- Auto-format code
- Train neural patterns
- Update memory
- Analyze performance
- Track token usage

### Session Management
- Generate summaries
- Persist state
- Track metrics
- Restore context
- Export workflows

## Advanced Features (v2.0.0)

- 🚀 Automatic Topology Selection
- ⚡ Parallel Execution (2.8-4.4x speed)
- 🧠 Neural Training
- 📊 Bottleneck Analysis
- 🤖 Smart Auto-Spawning
- 🛡️ Self-Healing Workflows
- 💾 Cross-Session Memory
- 🔗 GitHub Integration

## Integration Tips

1. Start with basic swarm init
2. Scale agents gradually
3. Use memory for context
4. Monitor progress regularly
5. Train patterns from success
6. Enable hooks automation
7. Use GitHub tools first

## Support

- Documentation: https://github.com/ruvnet/claude-flow
- Issues: https://github.com/ruvnet/claude-flow/issues
- Flow-Nexus Platform: https://flow-nexus.ruv.io (registration required for cloud features)

---

Remember: **Claude Flow coordinates, Claude Code creates!**

# important-instruction-reminders
Do what has been asked; nothing more, nothing less.
NEVER create files unless they're absolutely necessary for achieving your goal.
ALWAYS prefer editing an existing file to creating a new one.
NEVER proactively create documentation files (*.md) or README files. Only create documentation files if explicitly requested by the User.
Never save working files, text/mds and tests to the root folder.
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
