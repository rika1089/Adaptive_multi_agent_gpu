# Adaptive Multi-Agent GPU

A clean, paper-first implementation of **Adaptive GPU Resource Allocation for Multi-Agent Collaborative Reasoning**.

## Goal

This repository is being rebuilt from scratch to implement the base paper in a reproducible and academically defensible way.

The project is divided into four layers:

1. **Core simulation** – faithful implementation of the paper's adaptive GPU allocation logic.
2. **Experiment runner** – scripts to reproduce baseline comparisons.
3. **Monitoring/reporting** – metrics, result summaries, and figures.
4. **Optional deployment** – DGX / Docker / endpoint integration after simulation works.

## Planned comparison

The implementation will compare:

- Static allocation
- Round-robin allocation
- Adaptive allocation

using metrics such as:

- Latency
- Throughput
- GPU utilization

## Repository structure

```text
configs/        Experiment and agent configuration
docs/           Architecture and methodology notes
experiments/    Reproducible experiment entry points
scripts/        Helper shell scripts
src/            Main Python package
tests/          Unit tests
data/           Raw and processed workload inputs
output/         Logs, metrics, figures, and reports
```

## Current status

This repository currently contains the fresh project skeleton. The next steps are:

1. Add YAML configuration files
2. Implement baseline schedulers
3. Implement adaptive allocator
4. Build simulation environment
5. Add evaluation pipeline
6. Add optional DGX deployment layer

## Notes

The first milestone is **paper-faithful simulation**, not DGX deployment. Real-world deployment comes only after the allocator and experiment pipeline are validated.
