# Katherine Solano

**Product builder · AI agents · decision systems**

[getzona.app](https://getzona.app) · [LinkedIn](https://linkedin.com/in/katherinesolano)

I build products where software has to make or support real-world decisions. I'm the founder of ZONA, where I'm building nightlife infrastructure used by consumers, venues, and AI agents. My open-source work explores reliability and control in autonomous systems: Sentra decides whether an agent's action should be allowed to execute; Vigil independently verifies whether automated work actually produced the outcome it claimed.

## Selected Work

### ZONA

My company. Consumer nightlife discovery, venue and event data, table inventory and booking infrastructure, an AI Concierge, and an MCP layer that lets AI agents query ZONA's live nightlife data and, in supported cases, initiate table requests.

[getzona.app](https://getzona.app) · [AI infrastructure](https://getzona.app/ai)

### Vigil

**A job reporting success is a claim, not proof.**

Vigil wraps scheduled automation and independently verifies that the intended outcome actually occurred rather than trusting the job's own exit code.

- Separates what a job claims from independent evidence of the outcome
- Detects missed execution windows and catches up runs that never happened
- Detects degradation when a job remains alive but stops producing meaningful changes
- Supports independent verification through files, HTTP state, commands, and metrics

[github.com/ksolano220/vigil](https://github.com/ksolano220/vigil)

### Sentra

Sentra sits between an AI agent's decision and tool execution, evaluating proposed actions against deterministic policy before they are allowed to run.

- Deterministic runtime policy enforcement with no model in the decision loop
- Cumulative risk tracking per agent with three-strike shutdown
- Fail-closed Python SDK
- Structured audit events for evaluated actions
- Model-agnostic execution boundary

Started as an IBM SkillsBuild project. A healthcare adaptation, Sentra Medication, won the final pitch at NYU SPS's Berlin GFI.

[github.com/ksolano220/sentra](https://github.com/ksolano220/sentra) · [Live demo](https://sentra-demo.streamlit.app)

### Applied AI

**[Autonomous Claims Workflow](https://github.com/ksolano220/autonomous-claims-workflow)** — Multi-agent IBM watsonx/Granite system with Sentra at the tool-execution boundary.

**[Sentra Medication](https://github.com/ksolano220/sentra-medication)** — Healthcare adaptation of Sentra using FHIR-based patient context for medication-order governance.

**[Symptom Triage Coach](https://github.com/ksolano220/symptom-triage-coach)** — LoRA fine-tune of Qwen2.5-1.5B converting plain-language symptoms into schema-validated structured output using synthetic training data.

**[Symptom Triage Coach v2](https://github.com/ksolano220/symptom-triage-coach-v2)** — Multimodal image + text extension with an evaluation against the text-only baseline.

### Decision Systems & Analytics

**[Marketplace Pricing & Promotion Simulator](https://github.com/ksolano220/marketplace-pricing-promo-simulator)** — Contribution-margin decision simulator on 824K transaction line items, ranking which economic lever moves profitability most.

**[Care Gap Engine](https://github.com/ksolano220/care-gap-engine)** — Ranks open care gaps by clinical urgency, response likelihood, and equity priority.

[More analytics work →](https://github.com/ksolano220?tab=repositories)

## Sentra and Vigil

Sentra asks: **should this action be allowed to happen?**

Vigil asks: **did the automated work actually happen?**

One sits before execution. The other checks after. Neither treats self-reported success as sufficient evidence.

## How I Work

**Business problem → data → hypothesis → intervention → measurement → decision.**

I use code when it's the fastest way to test the hypothesis or operationalize the answer.

## Tools

Python · SQL · pandas · FastAPI · Streamlit · IBM watsonx · Hugging Face / PyTorch · LoRA fine-tuning · MCP · LLM evaluation · multi-agent systems

## Background

Founder, ZONA  
MBA, Pepperdine Graziadio  
M.S. Management & Analytics, NYU
