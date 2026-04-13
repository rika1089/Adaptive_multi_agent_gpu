
# Architecture

## Objective

This project implements the base paper's adaptive GPU allocation strategy for a four-agent multi-agent reasoning system.

## Main layers

1. Configuration layer (`configs/`)
2. Scheduling policy layer (`src/adaptive_gpu/scheduler/`)
3. Simulation layer (`src/adaptive_gpu/simulation/`)
4. Metrics and evaluation layer (`src/adaptive_gpu/metrics/`, `src/adaptive_gpu/evaluation/`)
5. Optional deployment layer (`src/adaptive_gpu/deployment/`)

## Agents

The planned four-agent system consists of:

- Coordinator
- NLP agent
- Vision agent
- Reasoning agent

## Policies

The repository will compare:

- Static allocation
- Round-robin allocation
- Adaptive allocation

## Principle

The project should first reproduce the paper in simulation before extending to real DGX deployment.
