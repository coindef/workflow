# Workflow Overview: Reezen (Agentic Causal Decision Intelligence Platform)

Reezen is an agentic decision-engineering system that transforms ambiguous, high-stakes strategic problems into structured decision specs and verifiable, evidence-backed recommendations.

## Architecture & Core Primitives

Reezen is built around two fundamental primitives designed to reduce black-box behavior and enable causal validation:

- **`DecisionContract` (Input Spec):** A typed specification defining objectives, constraints, risk thresholds, evidence requirements, and permissible interventions. It serves as the source of truth for the agentic workflow.
- **`DecisionArtifact` (Output Pack):** A persistent, searchable record of the decision logic, including assumptions, scenarios, simulation results, counterfactual tests, sensitivities/trade-offs, and the final recommendation.

## The Execution Loop

1. **Intent Synthesis:** Translate ambiguous user intent into a draft `DecisionContract`.
2. **Constraint Validation:** The user reviews and locks constraints and evidence requirements.
3. **Multi-Agent Orchestration:** Specialized agent roles generate candidate interventions, identify key uncertainties, and produce a test plan. Where useful, parallel agents explore competing assumptions and alternative framings.
4. **Simulation & Stress-Testing:** Candidate interventions are evaluated via simulation templates and counterfactual sweeps (sensitivities, boundary conditions, failure modes).
5. **Artifact Generation:** Produce a `DecisionArtifact` designed for auditability, search, and future replay.


[![Workflow Diagram](workflow.png)](workflow.png)

## License

Apache 2.0 - See [LICENSE](LICENSE) file for details.

## Support

For issues and questions:
- GitHub Issues: https://github.com/coindef/workflow/
- Documentation: See `/docs` directory
