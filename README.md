# Amazon Braket

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Amazon Braket is a fully managed quantum computing service that helps researchers and developers explore and build quantum algorithms, test them on quantum circuit simulators, and run them on different quantum hardware technologies. Braket provides access to multiple quantum processors from IonQ, Rigetti, QuEra, Oxford Quantum Circuits, and IQM, as well as high-performance simulators.

**Human URL:** [https://aws.amazon.com/braket/](https://aws.amazon.com/braket/)

**API Reference:** [https://docs.aws.amazon.com/braket/latest/APIReference/](https://docs.aws.amazon.com/braket/latest/APIReference/)

## APIs

### Amazon Braket API
Programmatic access to quantum task execution, device discovery, hybrid job management, and spending limit control.

**Base URL:** `https://braket.us-east-1.amazonaws.com`

#### Key Operations

| Operation | Description |
|---|---|
| CreateQuantumTask | Submit a quantum circuit to a QPU or simulator |
| GetQuantumTask | Monitor quantum task status and retrieve results |
| SearchQuantumTasks | Search quantum tasks by filters |
| CancelQuantumTask | Cancel a queued or running task |
| SearchDevices | Discover available QPU and simulator devices |
| GetDevice | Get device details and capabilities |
| CreateJob | Create a hybrid quantum-classical job |
| GetJob | Monitor hybrid job status |
| CancelJob | Cancel a running hybrid job |
| CreateSpendingLimit | Set QPU/simulator usage spending limits |

## Features

- **Quantum Task Execution** — Submit circuits to QPUs or simulators with results in S3
- **Hybrid Jobs** — Managed classical-quantum workloads with priority QPU access
- **Multiple QPU Providers** — IonQ, Rigetti, QuEra, Oxford Quantum Circuits, IQM via unified API
- **Quantum Simulators** — SV1 (state vector), DM1 (density matrix), TN1 (tensor network)
- **Device Discovery** — Search and filter available devices by type, status, and provider
- **Spending Limits** — Cost control for QPU and simulator usage
- **Pulse Control** — Low-level hardware access for advanced experimentation

## Use Cases

- **Quantum Algorithm Research** — Develop and test algorithms on simulators before QPU runs
- **Quantum Chemistry** — Molecular simulation with VQE hybrid algorithms
- **Quantum Optimization** — Combinatorial optimization with QAOA
- **Quantum Machine Learning** — Hybrid quantum-classical ML workflows

## QPU Providers

| Provider | Technology |
|---|---|
| IonQ | Trapped Ion (Aria 1, Aria 2, Forte 1) |
| Rigetti | Superconducting (Ankaa-3) |
| QuEra | Neutral Atom (Aquila) |
| Oxford Quantum Circuits | Superconducting (Lucy) |
| IQM | Superconducting (Garnet) |

## Artifacts

| Type | URL |
|---|---|
| OpenAPI Spec | [openapi/amazon-braket-api-openapi.yml](openapi/amazon-braket-api-openapi.yml) |
| JSON Schema (Task) | [json-schema/braket-task-schema.json](json-schema/braket-task-schema.json) |
| JSON Structure | [json-structure/braket-resource-structure.json](json-structure/braket-resource-structure.json) |
| JSON-LD Context | [json-ld/context.jsonld](json-ld/context.jsonld) |
| Spectral Ruleset | [spectral/ruleset.yml](spectral/ruleset.yml) |
| Capabilities | [capabilities/capabilities.yml](capabilities/capabilities.yml) |
| Vocabulary | [vocabulary/vocabulary.yml](vocabulary/vocabulary.yml) |
| Examples | [examples/](examples/) |

## Common Properties

| Type | URL |
|---|---|
| Documentation | [https://docs.aws.amazon.com/braket/](https://docs.aws.amazon.com/braket/) |
| SDK (Python) | [https://github.com/amazon-braket/amazon-braket-sdk-python](https://github.com/amazon-braket/amazon-braket-sdk-python) |
| Examples | [https://github.com/amazon-braket/amazon-braket-examples](https://github.com/amazon-braket/amazon-braket-examples) |
| Pricing | [https://aws.amazon.com/braket/pricing/](https://aws.amazon.com/braket/pricing/) |
| Blog | [https://aws.amazon.com/blogs/quantum-computing/](https://aws.amazon.com/blogs/quantum-computing/) |
| GitHub Organization | [https://github.com/amazon-braket](https://github.com/amazon-braket) |

## Maintainers

**Kin Lane** — [kin@apievangelist.com](mailto:kin@apievangelist.com)
