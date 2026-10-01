# Technology Stack and Open-Source Reference Repositories

This section tracks the most relevant components for building an AI-driven, end-to-end closed-loop drug discovery pipeline.

## A. Target identification and biological screening

- `https://github.com/Ishitta-Sarkar/computational-drug-discovery-platform`
- `https://github.com/Rollins1989/drugai-lite`
- `https://github.com/Aravind1080-hub/AI-Drug-Discovery-Assisstant`
- `https://github.com/agnishreddy/CBL-B-Inhibitor-Discovery-Using-AI-QSAR-Modeling-and-Structure-Based-Virtual-Screening`

These repositories illustrate the common path from target modeling to molecular prioritization using ML and structure-based drug discovery techniques.

## B. Molecular generation and scoring

- `https://github.com/Redomic/NeuThera-Drug-Discovery-Toolkit`
- `https://github.com/MorganCThomas/MolScore`
- `https://github.com/EdoardoGruppi/Drug_Design_Models`
- `https://github.com/amorehead/awesome-molecular-generation`
- `https://github.com/jaechanglim/CVAE`
- `https://github.com/lamm-mit/MoleculeDiffusionTransformer`

These are the most relevant references for candidate generation, multi-objective scoring, and generative chemistry workflows.

## C. Active learning and optimization

- `https://github.com/cosmic-hydra/zane`

This is the strongest practical reference for Gaussian-process active learning and Bayesian optimization loops.

## D. LIMS / ELN / assay data infrastructure

- `https://github.com/senaite/senaite.core`
- `https://github.com/elabftw/elabftw`
- `https://github.com/DIGI-UW/OpenELIS-Global-2`
- `https://github.com/miso-lims/miso-lims`

These systems provide the operational backbone for sample tracking, result recording, and evidence capture.

## E. Closed-loop / autonomous discovery systems

- `https://github.com/sidb5/BiotechOS-AI-Native-ClosedLoop-Predictive-Robotic-DrugDiscovery-Engine`
- `https://github.com/gotree94/AI-Drug-Discovery-Closed-Loop-Orchestration`
- `https://github.com/WinterWei22/OmniScientist`
- `https://github.com/jackysiupuichung/virtual-biotech-scientist`

These are the direct analogues for closed-loop discovery platforms and autonomous scientific workflows.

## F. Retrosynthesis and synthesis design

- `https://github.com/ibh4/ai4s-molecular-docking`

This repository includes route repair and synthesis-aware optimization patterns relevant to synthesis planning.

## G. Market-oriented references

- `https://github.com/api-evangelist/atomwise`
- `https://github.com/julief23/G4PT_2026`

These references are valuable for understanding how AI-native platforms position themselves in the discovery ecosystem.

## H. Overall recommendation

For a working proof-of-concept, the best stack is:

- design generation: `NeuThera` or `MolScore`-backed generative model selection
- active learning: `zane`
- lab data backbone: `senaite`
- ELN: `elabftw`
- orchestration: `BiotechOS` / `OmniScientist` as reference architecture
- synthesis-aware optimization: retrosynthesis / route planning via custom integration or external tools
