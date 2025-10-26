[![CI](https://github.com/bradsaucier/iterate-forward/actions/workflows/ci.yml/badge.svg)](https://github.com/bradsaucier/iterate-forward/actions/workflows/ci.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

# CS 250: Software Development Lifecycle Portfolio

**Author**  
Bradley Saucier, SMSgt, USAF (Ret.)  
B.S. Candidate, Computer Science (STEM Project Management), Southern New Hampshire University  
B.A., Columbia University  
A.A.S., Community College of the Air Force  

## Overview

This repository contains the final project artifact for SNHU CS 250: Software Development Lifecycle. The core academic deliverable is a Sprint Review and Retrospective analysis for the "SNHU Travel" Minimum Viable Product (MVP).

The SNHU Travel MVP was defined as a first release with only the core features required to learn from real users. The objective was clear: deliver a public booking flow for a curated travel package with secure payment and confirmation. The Product Goal and Sprint Goals were used to enforce that focus and prevent scope creep.

This repository also includes "The Controller's Compass" under `ethos/MONOGRAPH.md`. The monograph maps Combat Controller doctrine to Agile software delivery. It explains how Commander's Intent becomes Product Goal, how the OODA loop becomes sprint cadence, how PACE planning becomes resiliency under failure, and how AAR culture becomes Retrospective discipline. This is deliberate positioning. It shows that I execute software work using the same command mindset that drove combat control teams: clarity of mission, tempo, accountability.

## Core Artifact

The primary assignment deliverable is located in the `assignment/` directory:

- `./assignment/CS-250-Sprint-Review-Retrospective.pdf`

That document covers the Scrum execution model used on SNHU Travel:

- Five consecutive one week sprints on a fixed cadence
- Roles defined as Product Owner (PO), Scrum Master, Developers, and Tester
- Work pulled from a refined Product Backlog in thin vertical slices, aligned to INVEST (Independent, Negotiable, Valuable, Estimable, Small, Testable)
- Definition of Done (DoD) that required peer review, automated tests, Product Owner acceptance, performance validation, and security checks before anything was considered releasable

It also documents specific execution behaviors:

- Daily Scrum was held in a strict 15 minute timebox to synchronize and adapt the plan for the next 24 hours. The team walked the board right to left to focus on finishing work closest to Done before pulling anything new
- When payment integration ran into a vendor level blocker, the team adapted by swapping in a story of equivalent size to keep the Sprint Goal intact instead of letting the sprint fail. This protected delivery tempo under pressure
- The Scrum Master shielded the team from ad hoc, mid sprint work requests by redirecting them to the backlog. This preserved focus on the Sprint Goal. This was an explicit act of protecting Commander's Intent at the sprint level

The artifact in `assignment/` is the graded submission.

---

## CS 250 Journal Reflection (Essential Questions)

The following sections answer the required CS 250 Module Eight Journal questions. These answers are written as operational lessons learned, not theory. They also address instructor feedback by including both strengths and difficulties.

### 1. How do I interpret user needs and implement them into a program? How does creating "user stories" help with this?

Interpreting user needs is not guesswork. It is controlled translation from stakeholder intent into testable increments.

In this project, the Product Owner (PO) gathered client goals and market expectations, then expressed them as backlog items toward a Product Goal. The PO did not just collect requests. The PO shaped them into a focused Product Goal that defined what success looked like for the MVP booking flow and payment path.

User stories were the primary tool for conversion of that intent into executable work. User stories help in three specific ways:

1. Forcing clarity  
   Stories were refined to meet INVEST: Independent, Negotiable, Valuable, Estimable, Small, Testable. INVEST prevents vague, high level asks from entering a sprint. It forces the team to slice features into thin, verifiable chunks instead of trying to land entire subsystems at once.

2. Defining Done up front  
   A story does not mean anything without acceptance criteria. Acceptance criteria are the measurable contract between business intent and engineering output. The "Cruise Preference Toggle" story is a concrete example: its criteria covered accessibility, labeled controls, keyboard operability, sub one second performance, and persistent state. That level of detail makes the work objectively testable. There is no argument at Sprint Review about whether it is done.

3. Maintaining alignment on why  
   A good story ties the work to a user outcome, not just a task. This prevents gold plating and prevents "I built what you said, not what you meant." It also gives developers leverage to push back if requested work is not tied to real value.

Execution note  
The most important communication in Scrum did not happen in Daily Scrum. It happened in backlog refinement. Backlog refinement is where the PO, developer, and tester sat down and hammered acceptance criteria into something that was unambiguous, testable, and achievable. That is where risk was burned down. That is where misunderstanding was exposed and killed before it could cost a sprint.

### 2. How do I approach developing programs? What Agile processes do I hope to incorporate into my future development work?

My approach is iterative, feedback driven, and risk focused. I treat software delivery the way an assault force treats an objective: define intent, execute in short controlled pushes, assess, adapt, and push again.

Scrum provides that loop. Each one week sprint in this project acted like a mission cycle:

- Sprint Planning set the Sprint Goal. This is Commander's Intent for the next 5 workdays. It defines success conditions.
- Daily Scrum was a 15 minute tactical huddle to recheck alignment and surface blockers. The team walked the board from right to left and swarmed work that was nearly complete instead of starting new items. That is disciplined throughput, not busywork.
- Continuous Integration (CI) enforced Definition of Done with automated reviews, performance checks, and security scans on every code change. The DoD was not a suggestion. It was a gate.
- Sprint Review captured stakeholder feedback against a working increment every single week.
- Sprint Retrospective captured team level feedback and process adjustments.

This is the OODA loop in software:

- Observe: Gathering raw data. This is stakeholder reaction in Sprint Review and direct feedback from the working increment in front of them.
- Orient: Retrospective and backlog refinement, where the team analyzes what happened, what it means, and how it affects risk.
- Decide: Sprint Planning, where the Sprint Goal is chosen as the next tactical objective.
- Act: Sprint execution.

That loop is how you outpace risk. You do not wait 5 weeks to find out you were wrong. You find out in 5 days.

Processes I will continue using:

- Strict timeboxing. If an event is 15 minutes or 30 minutes, it ends on time. Time is the only non renewable resource in a one week sprint tempo. Discipline here prevents Scrum from becoming ceremony overhead instead of value.
- Definition of Done as a hard gate. The DoD in this project required peer review, automated test coverage, Product Owner acceptance, no performance regression, and passing security checks before calling any story Done. This prevents the quiet buildup of technical debt disguised as velocity.
- Sprint Goal protection. The Scrum Master in this project blocked mid sprint scope injections by redirecting them to the backlog. That preserves Commander's Intent and keeps the team aligned on objective instead of being yanked by noise.
- Swarming and board walk discipline. Work is finished before new work is started. That is how you keep throughput high and work in progress low.

### 3. What does it mean to be a good team member in software development?

Being a good team member is not about individual velocity. It is about accountable execution in support of the shared objective.

In practice that means:

- Proactive communication  
  The tester and developer did not wait to discover mismatched expectations on demo day. They used structured requests up front. Testers asked for error handling rules and expected error strings. Developers asked for Given-When-Then acceptance criteria and CI links before pulling a story. This is how ambiguity is killed before it burns a sprint.

- Upholding shared quality  
  Quality was not "QA's job." The DoD made quality the responsibility of the entire team: peer review, automated tests, performance checks, and Product Owner acceptance were required before a story could close.

- Swarming blockers  
  When a story was one step from Done, the team stopped opening new work and swarmed it to closure. The board was walked from right to left in Daily Scrum. This maximizes throughput and protects the Sprint Goal. It also builds habit discipline: finish what is in flight before starting something new.

- Disciplined adaptability  
  When a payment vendor issue blocked a story, the team did not let the sprint fail. They worked with the Product Owner to swap in an equivalent effort item after confirming it would still serve the Sprint Goal. That is controlled adaptation. That is not panic. That is not "change the plan because we are stuck." That is maintaining intent under friction.

Operational view  
A good team member is someone who treats the Sprint Goal like mission intent, treats ambiguity as a threat vector, and treats time as a limited resource that must be defended.

---

## Addressing Project Feedback

My instructor's feedback on the Sprint Review and Retrospective document was precise. The feedback was that I explained the mechanics of Scrum well, but I did not cover enough of the friction: communication challenges, overhead costs, and the cons of Scrum in a real sprint environment. The following points directly close those gaps and will remain part of this README for context.

1. Communication friction between technical and non technical roles  
   Challenge: A non technical Product Owner speaks in terms of business value. A developer and tester speak in terms of systems and constraints. If that gap is not closed, acceptance criteria come in weak or subjective and the team burns a sprint building something that technically works but does not actually solve the business problem.  
   Mitigation: Treat backlog refinement as a live alignment session instead of a passive handoff. The Product Owner owns the "what" and "why." The technical team is responsible for making sure acceptance criteria are unambiguous, testable, and feasible. The lesson: shared understanding is built before work starts.

2. Scrum ceremony overhead in a one week sprint  
   Challenge: At one week cadence, Sprint Planning, Daily Scrum, Sprint Review, and Sprint Retrospective consume a large percentage of total available working hours. If facilitation is weak, the team will feel like they are spending more time talking than executing.  
   Mitigation: Ruthless time discipline. Every event is timeboxed. Every event has a stated purpose and a clear output. Retrospective produces specific action items, not generic complaints. Lesson learned: The one week tempo is only sustainable if the Scrum Master enforces efficiency. Otherwise Scrum becomes drag instead of force multiplier.

3. Adaptability becoming avoidance  
   Challenge: Scrum gives the team the ability to adapt mid sprint. That adaptability can be abused. Teams can avoid the hardest work by swapping blocked or painful backlog items out for easier items, reporting a clean sprint while quietly deferring the real integration risk.  
   Mitigation: The Sprint Goal is the guardrail. You ask: did we adapt to overcome an obstacle, or did we adapt to avoid it. That question must be asked in Retrospective. Lesson learned: True agility is disciplined intent, not chaos. Adaptation that protects the mission is good. Adaptation that dodges the hard problem is corrosion.

4. Stress on quality caused by weak acceptance criteria  
   Challenge: If a story enters a sprint with vague or incomplete acceptance criteria, you cannot objectively test it at the end of the sprint. Quality becomes a debate, not a fact. That drives rework, churn, and mistrust.  
   Mitigation: Treat clear, testable acceptance criteria as a prerequisite to call a story ready. If criteria are not concrete, the story does not load. Lesson learned: The Definition of Done is the final gate, but acceptance criteria are the first gate.

Bottom line  
This reflection converts Scrum from a checklist into an operational model. It identifies not just how Scrum works when everything is clean, but what it costs to run Scrum at a one week tempo and what leadership behaviors are required to keep it honest.

---

## Repository Structure and Professionalization Layer

This repository is not only a course submission. It is an employment facing artifact. Its structure is intentional.

1. `assignment/CS-250-Sprint-Review-Retrospective.pdf`  
   The graded academic artifact for CS 250. This is the Sprint Review and Retrospective writeup for the SNHU Travel MVP. It documents Scrum execution, Definition of Done, backlog discipline, and cadence.

2. `ethos/MONOGRAPH.md`  
   "The Controller's Compass." This is a leadership doctrine statement. It maps Combat Controller processes to Agile software execution:
   - Commander's Intent maps to Product Goal and Sprint Goal. The Product Owner defines intent. The Scrum Master protects the team's ability to execute that intent without distraction.
   - OODA loop (Observe, Orient, Decide, Act) maps to iteration cadence. Sprint Review and daily feedback are Observe. Retrospective and backlog refinement are Orient. Sprint Planning is Decide. Sprint execution is Act.
   - PACE planning (Primary, Alternate, Contingency, Emergency) maps to resilience in systems and delivery. You design failover paths up front. You do not wait for a vendor API to fail and then improvise under panic.
   - AAR culture maps to Sprint Retrospective. The Retrospective is not a soft feelings session. It is an After Action Review focused on what happened, why it happened, and how to harden the system before the next iteration.

   Stated directly: I am not experimenting with Agile. I am applying battle tested command process to software delivery.

3. `.github/workflows/ci.yml`  
   A GitHub Actions workflow that automatically lints all markdown in the repo using markdownlint. This signals baseline CI discipline, even on documentation.

4. `.markdownlint.jsonc`  
   The markdownlint configuration file used by the CI workflow. This ensures consistent formatting and predictable review.

5. `.gitignore`  
   A professional grade .gitignore that prevents build artifacts, system files, virtual environments, node_modules, and IDE config from entering source control. This keeps the repo clean and inspection ready.

6. `LICENSE`  
   MIT License. This shows awareness of open source licensing norms and gives explicit terms of reuse.

7. `README.md`  
   The document you are reading now. It satisfies the CS 250 Module Eight Journal deliverable by answering the Essential Questions, addresses instructor feedback, and provides context for instructors and hiring managers.

---

## File Inventory and Intent

`README.md`  
Purpose: Executive summary. Satisfies CS 250 Module Eight Journal deliverable. Captures lessons learned, Agile execution, friction points, and leadership philosophy.  
Signal to employer: Shows communication discipline, ability to self-critique process, and ability to connect delivery work to mission level objectives.

`assignment/CS-250-Sprint-Review-Retrospective.pdf`  
Purpose: The original Sprint Review and Retrospective writeup for SNHU Travel.  
Signal to employer: Demonstrates working knowledge of Scrum roles, events, Definition of Done, backlog refinement, and delivery cadence under a one week sprint tempo.

`ethos/MONOGRAPH.md`  
Purpose: "The Controller's Compass." My leadership doctrine. Explains how Combat Controller mission execution maps to Agile software development and modern product delivery.  
Signal to employer: Establishes a unique value proposition. I can drive disciplined, iterative delivery under pressure, using a command mindset that emphasizes intent, tempo, resilience, and after action improvement.

`ethos/REFERENCES.md`  
Purpose: Source list backing "The Controller's Compass," including Agile doctrine, OODA theory, DevOps performance research, and modern delivery metrics.  
Signal to employer: Demonstrates that the leadership model is sourced, not buzzwords.

`.github/workflows/ci.yml`  
Purpose: GitHub Actions workflow that automatically lints markdown files for consistency and quality.  
Signal to employer: Shows baseline CI and automation mindset applied even to documentation.

`.markdownlint.jsonc`  
Purpose: Linter configuration consumed by the CI workflow.  
Signal to employer: Shows I am thinking about repeatability, consistency, and reviewability in version controlled artifacts.

`.gitignore`  
Purpose: Explicit control of tracked content. Keeps noise and environment specific artifacts out of the repo.  
Signal to employer: Shows professional source control habits.

`LICENSE`  
Purpose: MIT License covering the repository contents.  
Signal to employer: Shows understanding of IP control and open source norms.

End state  
This is a controlled, auditable portfolio artifact that shows not only what was delivered, but how it was delivered, what pressure points were encountered, and how those pressures were handled using disciplined execution principles. It is not classroom fantasy. It is applied process.

---

### Academic Integrity and Citation Policy

All work in this repository is my own, completed in accordance with the Southern New Hampshire University Academic Integrity Policy.  
