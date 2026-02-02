# Workflow Overview: Reezen (An Agentic Causal Decision Intelligence Platform)
Reezen is an agentic decision-engineering system that transforms ambiguous, high-stakes strategic problems into structured Decision Specs and verifiable, evidence-backed recommendations.

Architecture & Core Primitives
The architecture is built on two fundamental primitives designed to eliminate "black-box" and enable causal reasoning:
`DecisionContract` (Input Spec): A typed specification defining objectives, constraints, risk thresholds, and permissible interventions. It serves as the "source of truth" for the agentic workflow.
`DecisionArtifact` (Output Pack): A persistent, searchable record of the decision logic, including counterfactual scenarios, sensitivity analysis, and the final recommendation.

The Execution Loop
Intent Synthesis: Translates ambiguous user intent into a formal DecisionContract.
Constraint Validation: The user reviews and "locks" the contract's constraints and evidence requirements.
Multi-agent orchestration: specialized agent roles in a workflow to generate candidate interventions, identify key uncertainties, and produce a test plan. Where useful, parallel agents explore competing assumptions and alternative framings.
Simulation & Stress-Testing: Candidate interventions are subjected to counterfactual sweeps and simulation templates.
Artifact Generation: The system produces a comprehensive DecisionArtifact, designed for auditability, search, and future replay.

[![Workflow Diagram](workflow.png)](workflow.png)
