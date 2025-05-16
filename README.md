# member-extraction-algorithm-evaluation

This repository contains the code to evaluate the impact of the member extraction algorithm.
It compares the extraction of members between the extract-cbd-shape library, and the baseline extraction algorithm using a profile (optimum).

## Installation

```bash
npm install
npm run build
```

## Run

```bash
# Run as many client runners as you want, optionally on different machines.
npx ldes-evaluation-runner-client <name> <server-hostname>

# Run the benchmark orchestrator, this will start the benchmark and use the client runners.
npx ldes-evaluation-runner-orchestrator <env-file> <output-file> <hostname>
```

Alternatively, you can run the `run-benchmark.sh` script instead of the orchestrator.
This will start the benchmark and use the client runners for each configuration in the `config` directory.

```bash
npx ldes-evaluation-runner-client <name> <server-hostname>
./run-benchmark.sh <hostname>
```
