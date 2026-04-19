# Amazon Braket

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
