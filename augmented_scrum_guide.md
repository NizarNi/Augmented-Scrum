# The Augmented Scrum Guide
**For Human + AI Software Delivery Teams**
*Version 0.1 - Experimental*

---

## Purpose

Augmented Scrum extends Scrum to enable teams to build software safely and sustainably using AI-assisted development.

It addresses a new and critical reality:

> **AI accelerates code generation. It does not remove complexity. It converts it into entropy.**

Entropy - unpredictability, loss of structure, and loss of traceability - compounds faster than traditional technical debt. Left unmanaged, it makes systems unmaintainable, regardless of how quickly they were built.

The purpose of Augmented Scrum is to:
- Preserve human understanding of systems at all times
- Control the rate of AI-generated complexity
- Ensure the long-term evolvability of software

---

## Definition of Augmented Scrum

Augmented Scrum is a lightweight framework in which:

> **Humans design, control, and understand the system, while AI accelerates execution within constrained boundaries.**

Augmented Scrum does not replace Scrum. It governs the human–AI relationship within it.

---

## The Entropy Problem

AI coding tools introduce three interconnected forces that traditional Scrum does not address:

1. **Volume** — AI generates code faster than humans can understand it
2. **Opacity** — AI-generated decisions leave no traceable rationale
3. **Non-determinism** — AI can alter or remove system behavior without intent or warning

These forces produce **cognitive debt**: the progressive loss of the team's mental model of the system. Cognitive debt precedes technical debt. It makes technical debt invisible until it collapses.

> *"If no one on the team can explain the system, the system is not under control."*

---

## Core Principles

### 1. Human Ownership of the System
Humans are accountable for architecture, domain modeling, and all critical design decisions. AI must not define the structure of a system.

### 2. Controlled AI Autonomy
AI operates only within clearly scoped, bounded tasks. Unbounded AI generation is an unmanaged risk.

### 3. Entropy Must Be Actively Managed
Every iteration must include deliberate effort to reduce unpredictability, inconsistency, and loss of structure. Entropy does not manage itself.

### 4. Cognitive Sustainability
The system must remain understandable by humans at all times. Speed that destroys comprehension is not speed — it is deferred failure.

### 5. Validation Is a First-Class Activity
The primary bottleneck in AI-assisted development is not writing code. It is validating it. Validation must be planned, staffed, and measured.

---

## Accountabilities

### Product Owner
The Product Owner is accountable for:
- Maximizing product value over the long term, not just sprint velocity
- Defining requirements that are unambiguous, structured, and testable
- Ensuring AI receives clear, bounded inputs — not open-ended directives

### Augmented Developer
The Augmented Developer is a human professional accountable for:
- Maintaining a coherent mental model of the system
- Reviewing and validating all AI-generated code before integration
- Enforcing architectural consistency across iterations
- Ensuring every piece of code is understandable and safely modifiable
- Flagging entropy early — before it compounds

> The Augmented Developer is not a prompt engineer. They are the primary guardian of system integrity.

### AI Agent
The AI Agent is an execution tool that:
- Generates code, tests, or documentation within defined constraints
- Carries no accountability for system correctness or coherence
- Has no understanding of the system it modifies

> The AI Agent must never be treated as a team member. It has no judgment, no memory, and no responsibility.

---

## Artifacts

### Product Backlog
User stories and tasks must be structured and explicit enough for AI to execute within defined boundaries. Ambiguous items produce unbounded AI output.

### Sprint Backlog
Each Sprint Backlog must include three categories of work:
1. **Delivery work** — features and fixes
2. **Validation work** — human review of AI-generated output
3. **Entropy reduction work** — refactoring for comprehensibility, architecture alignment, cognitive debt repayment

No sprint is complete without all three.

### Increment
An Increment must satisfy two complementary standards:

#### Definition of Done (unchanged from Scrum)
- Functionality works as expected
- Tests pass
- Product is shippable

#### Definition of Control *(new in Augmented Scrum)*
- The code can be understood by a human in a reasonable time
- Design decisions are traceable and explainable
- System behavior is predictable
- The code can be safely modified in the next sprint

> **If the Increment meets the Definition of Done but fails the Definition of Control, it does not ship.**

---

## Events

### Sprint
A fixed-length iteration of one to four weeks. Every Sprint must produce:
- A validated, shippable Increment
- A measurable reduction in entropy

### Sprint Planning
The team defines:
- What will be built
- What AI is authorized to generate, and within what boundaries
- Who is responsible for validating each AI-generated component
- The cognitive budget for the sprint (see Rules)

### Daily Scrum
The focus shifts from activity reporting to system control:
- What was generated?
- What has been validated?
- What is not yet understood?

> *"I don't know" is a signal of entropy, not a scheduling problem.*

### Sprint Review
The Increment is evaluated for:
- Business value
- Stability and predictability
- Coherence and maintainability

Stakeholders must be informed of the current entropy level of the system.

### Sprint Retrospective
The team inspects:
- Was AI autonomy appropriately bounded?
- What caused cognitive overload this sprint?
- Did entropy grow, stay stable, or decrease?
- What will we constrain differently next sprint?

---

## Rules

### Rule 1 — AI Output Must Be Reviewable
No AI-generated code may be merged without a human who fully understands it. "I reviewed it quickly" does not satisfy this rule.

### Rule 2 — Cap AI Throughput to Human Validation Capacity
AI generation must be constrained to match the team's ability to review it. If the team cannot validate all output in the sprint, AI output must be reduced — not review standards.

### Rule 3 — Prefer Small, Bounded Changes
Large, opaque AI-generated changesets are prohibited. AI tasks must be scoped to produce reviewable increments of behavior.

### Rule 4 — Test Invariants, Not Permutations
Testing strategy focuses on system truths:
- What must always be true about this system?
- What must never happen?

Exhaustive permutation testing driven by AI non-determinism is unsustainable. Invariant testing is not.

### Rule 5 — Humans Own Architecture, Always
AI must not make decisions about:
- System structure
- Domain modeling
- Component boundaries
- Technology choices

These decisions belong to Augmented Developers. If AI has made them implicitly, the team must reclaim them explicitly.

### Rule 6 — Entropy Must Be Measured Each Sprint
The team must assess, at minimum qualitatively, whether entropy increased or decreased. If three consecutive sprints show entropy growth, the team must stop feature delivery and stabilize.

---

## The Cognitive Budget

Every sprint has a **Cognitive Budget**: the maximum volume of AI-generated change the team can fully understand in that sprint.

The Cognitive Budget is not a productivity ceiling. It is a sustainability floor.

Teams that exceed their Cognitive Budget consistently do not move faster. They accumulate invisible debt that surfaces as sudden, unrecoverable instability.

Suggested allocation per sprint:
- **50%** — delivery (features, fixes)
- **25%** — validation of AI-generated output
- **25%** — entropy reduction (comprehensibility, architecture, cognitive debt)

These ratios are starting points, not rules. Teams adjust based on their entropy level.

---

## What Augmented Scrum Is Not

- It is not a replacement for Scrum
- It is not an AI productivity framework
- It is not a set of prompting best practices
- It is not a tool recommendation

Augmented Scrum is an **entropy governance framework** for teams building software with AI assistance.

---

## Closing Statement

Scrum was designed for teams building software at human pace.

AI changes the pace. It does not change the responsibility.

> **Augmented Scrum exists to ensure that what teams gain in velocity, they do not lose in control.**

Software that cannot be understood cannot be maintained.
Software that cannot be maintained cannot evolve.
Software that cannot evolve has no long-term value.

The goal of Augmented Scrum is not maximum output.

It is **sustainable control over a system that grows.**

---

*The Augmented Scrum Guide is open for community contribution. Version 1.0 will be released following field validation across multiple AI-assisted delivery teams.*

*Authors: Nizar Louhichi, with contributions from the AI-assisted software delivery community.*
