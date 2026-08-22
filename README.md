# DEAP Profile: VHDL Hardware (`DEAP-profile-vhdl-hardware`)

> **Repository Role:** `PIPELINE_PROFILE_TEMPLATE` (VHDL Hardware Profile)  
> **Classification:** `FPGA / ASIC Hardware Design & Synthesis Platform Profile`  
> **Status:** `PRODUCTION-GRADE / ACTIVE`

---

## 1. Overview

The **DEAP VHDL Hardware Profile** (`DEAP-profile-vhdl-hardware`) provides hardware description, FPGA synthesis, RTL verification, and safety-critical hardware governance deliverables for the Digital Engineering Agent Platform (DEAP).

### 1.1 Primary Commercial Toolchain Integration Context

This project explicitly declares **MATLAB / Simulink / Stateflow / Embedded Coder** as the Primary Tier-1 Commercial Toolchain Integration Context (Model-Based Design, Control Law Synthesis, DO-178C C/SPARK Ada code generation).

---

## 2. Profile Structure & Governance

- `.agents/` & `AGENTS.md`: Agent behavior rules, role boundaries, and subagent dispatch protocols.
- `CLAUDE.md`: Claude Code guidelines and verification gates.
- `rules/`: Platform engineering rules and hardware design discipline rules.
- `schema/`: Contract definitions, interface schemas, and SysML v2 models.
- `scripts/`: Modular installer CLI and downstream verification scripts.
- `tests/`: Automated baseline verification test suite.

---

## 3. Verification & Quality Gates

Execute baseline verification:

```bash
# Run baseline tests
python3 -m pytest tests/

# Run downstream conformance gate
python3 scripts/verify_downstream_baseline.py --no-domain
```
