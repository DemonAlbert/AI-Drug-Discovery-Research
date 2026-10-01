# PRD 1: High-Throughput Rapid Iteration Pipeline

## 1. Product vision

Build a high-speed AI drug discovery system optimized for rapid iteration and parallel experimental feedback. The product is designed for teams that want to generate, assay, and learn from a high volume of molecules in compressed development cycles.

## 2. Product positioning

This product emphasizes:

- rapid batch generation
- multi-objective prioritization
- fast triage through core assays
- strong feedback loops between experimental results and model updates
- high throughput at the cost of some depth in each assay stage

## 3. Target users

- AI chemistry teams
- early discovery groups
- internal medicinal chemistry teams with access to CRO or automated assay infrastructure
- research teams pursuing a broad experimental search before narrowing to a lead series

## 4. Core user problem

Teams generate many compounds but struggle to turn those compounds into actionable biological insight quickly. Most existing systems either do heavy design but little experimental feedback, or do a lot of experimental work without enough decision intelligence.

## 5. Functional overview

### 5.1 Target and design layer
- disease target prioritization
- scaffold and chemical space definition
- AI candidate generation with diverse scaffolds
- multi-objective scoring across potency, novelty, feasibility, and ADMET risk

### 5.2 Assay and validation layer
- CRO protein expression and assay-readiness validation
- SPR and biochemical potency screens
- short-listing for selectivity and retained activity tests
- early ADMET and toxicity triage

### 5.3 Optimization layer
- active learning loop based on measured outcomes
- model update after each experimental batch
- design repair for compounds that fail in one stage but still show promise in another

### 5.4 Execution layer
- assay queue management
- automatic triage of batch runs
- result ingestion and quality control
- dynamic re-prioritization of next candidate batch

## 6. Key decision gates

- Gate A: target tractability and biological relevance
- Gate B: molecular feasibility and ADMET risk
- Gate C: protein expression and assay readiness
- Gate D: SPR engagement and biochemical potency
- Gate E: preserved activity / selectivity test
- Gate F: synthesis feasibility and route planning

## 7. Value proposition

This system enables teams to:

- shorten the time from design to experimental learning
- reduce dead-end chemistry cycles
- use observed wet-lab results to update model priorities in near-real time
- maintain a broad candidate pool while still filtering aggressively

## 8. KPI targets

- increase hit discovery throughput
- reduce time to first meaningful assay feedback
- maintain a high learning rate from each experimental batch
- improve candidate conversion from initial design to confirmed hits

## 9. Risks

- noisy assay data can lead to unstable model updates
- overemphasis on throughput may cause shallow validation of second-order effects
- early success can create false confidence without strong selectivity and ADMET filtering

## 10. Recommended deployment strategy

Start with a closed loop over a single disease area and a limited biological space. Use a narrow but representative target set and a moderate assay batch size. The first milestone is not to maximize scale; it is to prove the loop works end to end.

## 11. Product summary

This PRD is best suited for a team that wants to move quickly and learn from many experimental outcomes. It prioritizes speed, learning rate, and operational throughput.
