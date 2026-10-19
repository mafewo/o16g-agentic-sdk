# o16g Agentic SDK

Governance and orchestration framework for autonomous development driven by Artificial Intelligence agents.

## Philosophy
The goal is to transform software development from an artisanal process ("Vibe Coding") into an automated, measurable supply chain centered on business impact. Under the o16g framework, outcome engineering dictates that software is no longer the end goal, but rather a means to achieve a measurable impact.

## SDK Consumption (AGENTS.md Integration)
This repository functions as a "Central Brain". For any microservice or satellite project to inherit these rules, do not copy the files manually. Instead, use the `AGENTS.md` standard in the target repository and run the following initialization command to fetch `AGENTS.md`, the core rules, and the bootstrapping script:

```bash
mkdir -p scripts && curl -sL https://raw.githubusercontent.com/MadMorris/o16g-agentic-sdk/main/scripts/o16g -o scripts/o16g && chmod +x scripts/o16g && scripts/o16g init
```

The new `o16g` CLI tool streamlines initialization, canvas status checking, and structural pruning. It also installs a local Git pre-commit hook that validates the presence and state of `.o16g_state.md`.

Each satellite project can then extend these base rules with its own local overrides inside `.o16g/`, while the core governance always points back to this central repository. Furthermore, GitHub Actions and Templates are included for Automated PR verification enforcing Review-Driven Development (RDD).

---

## Documentation and Citations
The framework specifications use precise ontological markers (e.g., `[cite: 722]`) to ground assertions in the official o16g core. To explore the origins and definitions of these codes, refer to the [o16g Ontological Reference Library](docs/research/citations.md).
