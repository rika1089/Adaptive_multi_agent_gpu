# Methodology

## Phase 1: Paper-faithful implementation

- Define four agents and their priorities
- Define minimum GPU shares
- Generate synthetic workloads
- Implement three policies:
  - Static
  - Round-robin
  - Adaptive
- Compare latency, throughput, and utilization

## Phase 2: Evaluation

- Run reproducible experiments
- Save logs, metrics, and figures
- Compare results across policies

## Phase 3: Optional real-world execution

- Map simulation agents to real model endpoints
- Add DGX / Docker integration
- Validate whether the adaptive logic still helps in real deployment

## Important constraint

Real-world deployment is not the first milestone. The first milestone is simulation fidelity to the paper.
