# Systems, measurements and evidence boundaries

## Operating experience

An October 2026 inspection found a Pop!_OS environment with local models, Docker
applications, PostgreSQL, Redis, managed services and remote access. Internal source
includes media workflows, approval controls, queues, retries and dashboards.
Running services and source inspection support these descriptions; they do not
establish that every application path works end to end.

Recovery work includes encrypted snapshots and database restore tooling.
Historical records document isolated restore exercises and a controlled update
with rollback preparation and service checks. Those exercises were not repeated
for this portfolio. A later check matched an encrypted backup across two machines;
this confirms matching copies, not successful decryption or restoration.

Committed hardening work addresses concurrent state writes, duplicate actions and
credential exposure in command arguments. These are internal engineering examples;
no customer endorsements or third-party security certification are claimed.

## Local-AI experiment and subsequent review

Four fictional records supported four factual questions. A fifth question had no
matching record and was rejected by retrieval without calling the model. This
tests a small pipeline, not the model's independent refusal behavior.

Automated checks looked for expected terms, source selection and citation format.
All five passed in both completed runs. Later review found that one policy answer
reversed who gives notice while retaining the expected duration and citation.
That is a false positive in the test criteria. Five semantically correct answers
and general accuracy have not been established.

Before customer acceptance, testing should cover who takes an action, conditions,
exceptions and unsupported questions that share words with the records. Customer
examples should be separate from the examples used during development.

## Performance observations

Each completed run generated four model answers. The first included model loading;
the following three supplied the warm median and range. Operating-system cache
state was not controlled. No repeated trials, concurrency or sustained-load tests
were performed, so the first-answer difference is not a verified cold-start gain.

Loaded sizes are runtime observations, not independently measured peak memory.
The initial footprint was sampled in a separate request; the compact footprint
was sampled after its completed run. That limits direct comparison. An automatic
acceleration attempt failed during inference and was excluded from passing results.

## Inspectable and private evidence

[results.json](results.json) contains aggregate measurements and the hash of the
retained private compact-run report. The hash identifies that report if reviewed
later; the hash alone does not independently verify these claims.

Source, prompts, fixture contents, deployment settings, operational logs and private
business data are not published. A walkthrough can demonstrate selected behavior
without transferring these materials.

## Technical walkthrough agenda

1. Show the Linux environment and explain the relevant services.
2. Demonstrate an agreed synthetic task, attribution and a failure case.
3. Explain the observed model-loading and memory tradeoffs.
4. Walk through a sanitized recovery example and its verification limits.
5. Map customer requirements to deliverables and acceptance checks.

This is a walkthrough outline, not a recording or independently witnessed test.
