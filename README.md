# Local AI & Linux Systems — Jhay Foreign

**Local AI, business automation, and documented handoff for systems you own.**

I own a recording studio and label, and have built an internal Linux and AI
environment to support those operations. That work includes local inference,
containerized applications, custom media workflows, approval controls, dashboards,
and encrypted recovery tooling.

This portfolio connects that operating experience to a proposed offline knowledge
mini-PC project. Implementation source and internal business records remain private.

[Systems and evidence](EVIDENCE.md) · [Prototype delivery plan](DELIVERY.md) ·
[Measured results](results.json)

## What I have built and operate

| System | Relevant work | Value for your project |
|---|---|---|
| Linux / local AI environment | Pop!_OS, local models, Docker applications, PostgreSQL, Redis, managed services and remote administration | Integrating services on an existing Linux machine |
| Media automation | Python workflows, media processing, job queues, retries, approval controls and dashboards | Connecting tools into manageable business workflows |
| Recovery and maintenance | Encrypted database/configuration backups, restore tooling and documented update procedures | Planning for maintenance and recovery |
| Reliability improvements | Concurrent-state handling, duplicate-action prevention and secret-aware automation | Addressing operational failure modes |

These systems serve my own operations. The evidence page distinguishes inspected
components, historical records, and newly measured results.

## A practical approach to an offline knowledge mini PC

The proposed prototype combines local AI, reference and educational content,
a local portal, and repeatable setup and update instructions.

| Stage | Customer deliverable | Proposed acceptance check |
|---|---|---|
| Scope and base system | Hardware/content requirements, service layout and installation plan | Confirm storage, model fit, access and offline tasks |
| Integrated prototype | Container configuration, AI interface, content services and portal | Exercise user tasks, service startup and local access |
| Offline verification | Results for disconnected operation and failure recovery | Disconnect external connectivity, reboot and repeat agreed tasks |
| Handoff | Project repository, setup/update scripts, operator guide and walkthrough | Repeat installation on agreed clean hardware or a suitable test environment |

The offline content services would be new integrations into my existing skill set.
The [delivery plan](DELIVERY.md) explains the components and scoping questions.
Each stage has a review point and a concrete deliverable.

## Measured example: local knowledge answering

A compact AMD Linux system with 32 GB RAM ran a synthetic knowledge exercise.
Two configurations completed the exercise; a failed acceleration attempt was
also retained as evidence.

| Observation | Initial run | Compact run |
|---|---:|---:|
| Automated fixture checks passed | 5/5 | 5/5 |
| First answer, including model loading | 24.31 s | 11.21 s |
| Median of three subsequent answers | 5.43 s | 6.32 s |
| Runtime-reported loaded size | 17 GB | 9.4 GB |

The compact run used less reported memory, with slower subsequent answers. These
are single-run observations, not controlled cold-start benchmarks. The five checks
cover expected terms, source selection and citation formatting. A later review
found a wording error those checks missed; they are not a general accuracy score.
Read the [method and review notes](EVIDENCE.md).

## Discuss your prototype

Reply to the introduction that brought you here with your target hardware,
required content, expected user count, and tasks that must work offline.
I can use those requirements to propose milestones, a timeline and a project price.

A technical walkthrough can cover the operating environment, selected automation
and recovery examples, measured AI behavior, and the proposed delivery plan.
Existing business code stays private. Project-specific configuration, scripts and
documentation would be delivered under agreed scope and ownership terms.

Updated October 2026. [Rights and source availability](NOTICE.md).
