# The Controller's Compass

**Author**  
Bradley Saucier, SMSgt, USAF (Ret.)

## Introduction: The Point of Control

The radio was wet and the net was crowded. A-10s were inbound with different fuel states. An MQ-9 needed routing across a no-fire line. The ground force was pushing through a wadi under broken comms. Weather rolled in, winds aloft shifting. One hand on a grease pencil map, the other on a handset. The job is not to be the hero. The job is to make a system out of chaos. Take in the picture, orient on what matters, make the next call, and check effects. Then do it again. The cycle never stops.

Thesis. The tools we used to survive and succeed in that environment are not military secrets. They are general solutions to managing complexity. In software and product work the same answers show up with different names. Elite teams converge on the same doctrine because they face the same problems. Ground truth changes faster than any rigid plan.

## The Great Misunderstanding: Why Old Plans Fail In New Fights

The old military comfort was a linear plan. Phase lines, staff estimates, and a neat critical path. It works when the world holds still. It fails when the enemy votes and weather shifts. Software did the same under a strict sequence of requirements, design, build, test, deploy. The industry labeled it Waterfall, often stripped of the feedback Royce described in 1970. The economic failure mode is simple. In a long, sequential process, the cost to correct a wrong assumption climbs the later you find it. Errors compound across documents, interfaces, and schedules. The result is overruns, slips, and mismatched outcomes. The lesson is not panic. It is to stop applying a single-pass model to a high-change fight.

## The Four Pillars Of Elite Execution

### 1. Commander's Intent -> Product Vision

Anecdote. The commander did not hand me a script. He gave me purpose, key tasks, and end state. Example: establish an observation post on the ridge before sunrise to protect the main force's flank. Keep the team safe. The route, sensors, timings, and contingency plan were on us. The why drove the how. When comms dropped, intent kept us moving.

Principle. Commander's Intent pushes decision rights down to where the facts live. It reduces cognitive bottlenecks. It expects disciplined initiative within boundaries. The aim is speed and alignment.

Translation. In Scrum and modern product practice, Product Vision and a Product Goal set direction and value. Product defines the why and what. The team owns the how. The mechanism is the same tool in different clothes.

### 2. Observe-Orient-Decide-Act -> The Sprint Engine

Anecdote. In a short, violent contact you do not call a meeting. Muzzle flash in a window. Observe. Terrain, fields of fire, friendlies, civilians. Orient. Choose suppressive fire and a bounding move. Decide. Execute. Act. Brass hits the ground and the next observation starts. Faster cycles win.

Principle. The Observe-Orient-Decide-Act cycle is a continuous loop. The winner turns the loop faster and with better orientation than the threat.

Translation. Agile sprints are an organizational OODA loop. Review is Observe. Retrospective and refinement are Orient. Sprint planning is Decide. The sprint is Act. Continuous Integration and Continuous Delivery compress Act and speed up Observe by shipping small changes often. That is not automation for its own sake. It is a weapon that shortens the decision cycle.

### 3. PACE Planning -> Resilient Systems

Anecdote. For aircraft comms we had Primary, Alternate, Contingency, Emergency. Primary might be encrypted satellite. Alternate could be line-of-sight relay. Contingency was a scheduled runner to a vantage point. Emergency was a rally point if the world went dark. You do not invent this under fire. You rehearse it in daylight.

Principle. PACE is structured pessimism. It assumes friction and plans to absorb it. It keeps critical functions alive when the primary path fails.

Translation. In modern systems, Primary is a hardened, automated pipeline and a production region. Alternate is cross-zone or cross-region failover. Contingency is graceful degradation with essential services only. Emergency is a static status page, a rollback, and a drilled incident plan. Mean Time To Restore is the scoreboard.

### 4. After-Action Review -> The Retrospective With Teeth

Anecdote. After every mission we stripped rank at the door. Four questions, every time. What was supposed to happen. What actually happened. Why the delta. What we change next. One or two actionable changes leave the room. The newest airman could call out the team lead, and that was expected.

Principle. The AAR is a blame-free, fact-first learning loop. It hardwires humility and improvement.

Translation. Many retros drift into opinions. Fix that by anchoring to the sprint goal, accepted work, and objective data. Use deployment frequency, lead time, change fail rate, and time to restore service. Compare plan to outcome. Change one or two behaviors. Repeat.

## Synthesis: The Compass In Action

Scenario. A 90-day market entry.

- Intent. Leadership sets purpose and end state. Secure a beachhead user segment. Prove repeatable value by month three. Guardrails and ethics are explicit.
- OODA. Sprint 1 is recon. Ship a minimum viable product to an instrumented cohort. Observe behavior. Orient on signals. Decide the next slice. Act in Sprint 2. Keep cycle time short.
- PACE. Primary pipeline is automated to a multi-AZ environment. Alternate is a verified runbook for semi-manual deploys. Contingency degrades non-critical features under load. Emergency rollback and a status page are prepped and drilled.
- AAR. End of each sprint, compare goal to delivered. Review metrics and incidents. Make one or two changes. Over time MTTR drops and change fail rate falls while throughput rises.

## Conclusion: It Is Not The Plan. It Is The Planning

In warfare and technology the enemy is uncertainty. No single plan survives contact. The edge is not a thicker binder. It is a faster, truer learning loop executed by a team with decentralized judgment and rehearsed resilience.

Action. Stop chasing perfect plans. Build intent. Run your loop with data. Install PACE in architecture and drills. Conduct AARs that change behavior. That is the competitive edge in any complex fight.

## References

See the pinned citations and permalinks in [REFERENCES.md](./REFERENCES.md).
