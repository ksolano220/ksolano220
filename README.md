# Katherine Solano

**MBA Marketing, Pepperdine University | MS Data Analytics, NYU (in progress)**

Healthcare analytics, operational systems, and applied AI focused on workflow reliability, clinical decision support, and high-stakes environments.

## Currently

- Shipped [**Symptom Triage Coach v2**](https://github.com/ksolano220/symptom-triage-coach-v2). Multi-modal extension of the v1 LoRA fine-tune: image of the affected area plus a plain-language symptom in, image-grounded triage JSON out. Side-by-side eval comparing image+text vs text-only. [Live demo](https://symptom-triage-coach-v2.streamlit.app/).
- Just shipped [**Care Gap Outreach Engine**](https://github.com/ksolano220/care-gap-engine). Finds patients overdue for screenings, ranks who to contact first, and drafts the outreach with Claude. For clinics on HEDIS or value-based care contracts.
- Founder of [ZØNA](https://www.getzona.app), real-time decision platform that analyzes user behavior and demand to drive nightlife discovery. Leading product, design, and engineering across iOS and Android consumer apps, venue CRM, ads marketplace, and promoter portal. 100K+ downloads, paying venue partners, live since June 2024.
- Completed the **IBM SkillsBuild AI Experiential Learning Lab (2026)**. Built a multi-agent public-benefits workflow on IBM watsonx.ai + Granite, paired with a runtime execution control layer ([Sentra](https://github.com/ksolano220/sentra)) I built independently to govern it.

## Featured work

<table>
<tr>
<td width="50%" valign="top">
<a href="https://care-gap-engine.streamlit.app">
<img src="https://raw.githubusercontent.com/ksolano220/care-gap-engine/main/docs/dashboard.png" width="100%" alt="Care Gap Outreach Engine: prioritized queue with score breakdown, filters, and equity context"/>
</a>
<p><strong>care-gap-engine</strong><br/>
Population health outreach prioritization for primary care teams on value-based care contracts. Ranks open care gaps by clinical urgency × response likelihood × equity priority, then drafts personalized outreach with Claude. <a href="https://care-gap-engine.streamlit.app">Live demo</a>.</p>
</td>
<td width="50%" valign="top">
<a href="https://symptom-triage-coach-v2.streamlit.app/">
<img src="https://raw.githubusercontent.com/ksolano220/symptom-triage-coach-v2/main/docs/demo.png" width="100%" alt="Symptom Triage Coach v2: image-grounded triage output with visual findings, body systems, possible causes, red flags, and follow-up questions"/>
</a>
<p><strong>symptom-triage-coach-v2</strong><br/>
Multi-modal pre-visit triage. Image of the affected area plus a plain-language symptom in, schema-valid triage JSON out with image-grounded visual findings. <a href="https://symptom-triage-coach-v2.streamlit.app/">Live demo</a>.</p>
</td>
</tr>
</table>

## Projects

### Applied AI

**[symptom-triage-coach-v2](https://github.com/ksolano220/symptom-triage-coach-v2)** · [live demo](https://symptom-triage-coach-v2.streamlit.app/)
Multi-modal extension of the v1 fine-tune. Takes an image of the affected area plus a plain-language symptom description and returns a structured triage JSON with image-grounded visual findings, ranked possible causes, red flags, and pre-visit questions. Built on Claude Sonnet 4.6's vision API with jsonschema-validated output. Side-by-side eval harness compares image+text vs text-only output across consistent, vague-text, and text-image-conflict cases.

**[symptom-triage-coach](https://github.com/ksolano220/symptom-triage-coach)** · [live demo](https://huggingface.co/spaces/ksolano220/symptom-triage-coach)
LoRA fine-tune of Qwen2.5-1.5B that converts a plain-language symptom into a structured pre-visit prep response: body systems, ranked possible causes, red flags, questions to prepare for. Schema-valid JSON output eliminates the hallucinated medical statistics that were the failure mode of an earlier Cochrane-based iteration ([plain-english-medicine](https://github.com/ksolano220/plain-english-medicine)). Full pipeline from synthetic data generation (GPT-4o-mini teacher) through QLoRA training on a T4 to a live Gradio Space.

**[sentra](https://github.com/ksolano220/sentra)** · [live dashboard](https://sentra-demo.streamlit.app)
Runtime execution control layer for autonomous AI agents. Intercepts proposed actions, scores cumulative risk, and enforces allow, block, or shutdown decisions before execution. Model-agnostic: no LLM SDK dependencies.

**[autonomous-claims-workflow](https://github.com/ksolano220/autonomous-claims-workflow)** · [live demo](https://ksolano-claims.streamlit.app/)
The proof-of-concept that validated Sentra. A multi-agent public-benefits workflow built on IBM watsonx.ai + Granite for the IBM SkillsBuild AI Experiential Learning Lab (2026), completed as a solo submission. The claims agents intentionally propose unsafe actions (approving payouts without verification, exfiltrating data). Sentra sits at the tool-execution boundary and blocks them before they run. Together, the two repos demonstrate the runtime-governance pattern end-to-end.

**[cortex](https://github.com/ksolano220/cortex)** · [live dashboard](https://ksolano-cortex.streamlit.app/)
Dual-model governance system where two AI models review each other's work. Worker writes, overseer stress-tests, debate runs until output passes your rules. Self-healing agents respawn with memory after repeated failures. Includes an opt-in executor that applies approved worker output to a workspace with path-traversal and denylist safety rails.

### Healthcare Analytics

**[care-gap-engine](https://github.com/ksolano220/care-gap-engine)** · [live demo](https://care-gap-engine.streamlit.app)
Detects open care gaps over a 1,000-patient synthetic panel using USPSTF and HEDIS rules, then ranks them by clinical urgency, likelihood-to-respond, and equity priority. Drafts personalized outreach per top-priority patient with Claude. Streamlit dashboard with prioritized queue, equity breakdown, and methodology card.

**[medicare-billing-analysis](https://github.com/ksolano220/medicare-billing-analysis)**
SQL analysis of 145,000 CMS Medicare records across 3,000+ hospitals. Surfaced billing markups exceeding 400% of national averages and quantified rural vs urban care delivery gaps.

**[ed-wait-time-dashboard](https://github.com/ksolano220/ed-wait-time-dashboard)** · [live demo](https://ksolano220-ed-wait-times.streamlit.app/)
Streamlit dashboard benchmarking emergency department wait times across 4,000+ US hospitals with state-level comparisons.

**[healthcare-access-risk-analysis](https://github.com/ksolano220/healthcare-access-risk-analysis)** · [live map](https://ksolano220.github.io/healthcare-access-risk-analysis/)
County-level risk scoring for 3,200+ US counties using uninsured population data and hospital density. Interactive Folium choropleth for resource planning.

**[clinical-trial-trends](https://github.com/ksolano220/clinical-trial-trends)** · [live demo](https://clinical-trial-trends.streamlit.app)
Exploratory analysis of 10,000 ClinicalTrials.gov trials. Sponsor patterns, phase completion rates, and geographic distribution. Interactive Streamlit dashboard with filters by phase, sponsor type, year, and condition keyword.

## Skills

- **Data:** SQL, Python (pandas, NumPy), data modeling, ETL
- **Healthcare:** HIPAA-aware data handling, HEDIS / USPSTF rule logic, CMS and claims data, value-based care, FHIR / EHR concepts
- **Analysis:** exploratory analysis, cohort analysis, A/B testing, risk scoring
- **Visualization:** Streamlit, Plotly, matplotlib, Folium, Tableau
- **Applied AI:** LoRA / QLoRA fine-tuning, Hugging Face Transformers, PyTorch, multi-agent systems, IBM watsonx.ai / Granite
- **Backend:** Node.js, Express, MongoDB, Firebase, FastAPI
- **Product:** iOS, React Native, user research, design systems

## Contact

- LinkedIn: [linkedin.com/in/katherinesolano](https://www.linkedin.com/in/katherinesolano)
- New York, NY
