# Local AI Feasibility Case Study

Private implementation, public results. Prepared by Jhay Foreign in October 2026.

## Objective

Determine whether a compact Linux computer can answer operational questions from
a small local knowledge set, cite the selected record, reject an unsupported
question, and produce evidence suitable for a deployment decision.

The implementation, prompts, synthetic fixtures, internal operating records, and
source code remain private. This repository is an evidence-only case study.

## Tested environment

- Pop!_OS on a compact AMD Ryzen 9 PRO system
- 32 GB system memory and integrated AMD graphics
- A local quantized model served through a loopback-only inference endpoint
- Fictional test records; no customer, artist, label, or production data
- No paid API, cloud inference, or new hardware used for the test

## Acceptance criteria

Five predefined cases were evaluated:

1. Retrieve and cite an emergency-contact record.
2. Retrieve and cite a scheduling-policy record.
3. Retrieve and cite a data-retention record.
4. Retrieve and cite a warranty record.
5. Reject a question not supported by the supplied records.

Passing required the expected source, expected fact, and source citation for each
supported question. The unsupported question had to return the defined refusal.

## Results

| Measurement | Initial configuration | Selected compact configuration |
|---|---:|---:|
| Acceptance cases passed | 5/5 | 5/5 |
| Cold first answer | 24.31 s | 11.21 s |
| Warm-answer median | 5.43 s | 6.32 s |
| Warm-answer range | 5.07–6.10 s | 5.84–7.13 s |
| Runtime-reported loaded size | 17 GB | 9.4 GB |

The selected configuration reduced the displayed loaded size and cold-start time,
with a modest warm-response tradeoff. One automatic acceleration configuration
failed during inference and was rejected rather than counted as a successful run.

The aggregate machine-readable result is in [results.json](results.json). Its
`private_artifact_sha256` value identifies the retained private raw report without
publishing the report, fixtures, prompts, or implementation.

## What this establishes

- One bounded local knowledge workflow ran successfully on the tested hardware.
- Performance and failure behavior were measured instead of inferred.
- A smaller runtime footprint was achievable without losing the five-case result.
- The test can support a scoped feasibility discussion and deployment estimate.

## What this does not establish

This is not proof of production accuracy, complete offline behavior, security
certification, access control, high concurrency, large-document retrieval, or
performance on customer data. The client application used a loopback endpoint,
but the operating system and model runtime were not independently network-audited.

## Commercial scope demonstrated

The evidence supports a small first milestone: hardware and software inventory,
one synthetic-data workflow, measured latency and task success, documented failure
cases, and a handoff describing whether a larger deployment is justified.

It does not claim a finished platform, custom model training, penetration testing,
regulatory compliance, or 24/7 managed support.

## Rights and source availability

No source code or implementation license is granted through this repository. See
[NOTICE.md](NOTICE.md). Technical details may be discussed under an agreed project
scope without transferring unrelated proprietary systems or operating records.
