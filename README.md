# Katherine Solano

**MBA Marketing, Pepperdine University | MS Data Analytics, NYU (in progress)**

Data analyst and product builder. I ship applied-AI work with a bias toward projects that answer the "so what" question and deliver something someone can actually use.

## Currently

- **Open to full-time roles in Applied AI / ML engineering or data analytics**, New York-based or remote. Healthcare tech is a specialty, not a requirement.
- Founder of [Zona](https://www.getzona.app), a real-time nightlife decision app for iOS.
- Completed the **IBM SkillsBuild AI Experiential Learning Lab (2026)** as a solo submission. Built a multi-agent public-benefits workflow on IBM watsonx.ai + Granite, paired with a runtime execution control layer ([Sentra](https://github.com/ksolano220/sentra)) I built independently to govern it.

## Featured work

[![Symptom Triage Coach LoRA fine-tune output](https://raw.githubusercontent.com/ksolano220/symptom-triage-coach/main/outputs/demo.png)](https://huggingface.co/spaces/ksolano220/symptom-triage-coach)

LoRA fine-tune of Qwen2.5-1.5B that turns a patient's plain-language symptom into a structured pre-visit prep response. [Try the live demo.](https://huggingface.co/spaces/ksolano220/symptom-triage-coach)

## Projects

### Applied AI

**[symptom-triage-coach](https://github.com/ksolano220/symptom-triage-coach)** · [live demo](https://huggingface.co/spaces/ksolano220/symptom-triage-coach)
LoRA fine-tune of Qwen2.5-1.5B that converts a plain-language symptom into a structured pre-visit prep response: body systems, ranked possible causes, red flags, questions to prepare for. Schema-valid JSON output eliminates the hallucinated medical statistics that were the failure mode of an earlier Cochrane-based iteration ([plain-english-medicine](https://github.com/ksolano220/plain-english-medicine)). Full pipeline from synthetic data generation (GPT-4o-mini teacher) through QLoRA training on a T4 to a live Gradio Space.

**[sentra](https://github.com/ksolano220/sentra)**
Runtime execution control layer for autonomous AI agents. Intercepts proposed actions, scores cumulative risk, and enforces allow, block, or shutdown decisions before execution. Model-agnostic: no LLM SDK dependencies. [autonomous-claims-workflow](https://github.com/ksolano220/autonomous-claims-workflow) is the IBM watsonx.ai proof-of-concept that integrates Sentra at the tool-execution boundary.

**[cortex-2c](https://github.com/ksolano220/cortex-2c)**
Dual-model governance system where two AI models review each other's work. Worker writes, overseer stress-tests, debate runs until output passes your rules. Self-healing agents respawn with memory after repeated failures. Includes an opt-in executor that applies approved worker output to a workspace with path-traversal and denylist safety rails.

### Healthcare Analytics

**[medicare-billing-analysis](https://github.com/ksolano220/medicare-billing-analysis)**
SQL analysis of 145,000 CMS Medicare records across 3,000+ hospitals. Surfaced billing markups exceeding 400% of national averages and quantified rural vs urban care delivery gaps.

**[ed-wait-time-dashboard](https://github.com/ksolano220/ed-wait-time-dashboard)** · [live demo](https://ksolano220-ed-wait-times.streamlit.app/)
Streamlit dashboard benchmarking emergency department wait times across 4,000+ US hospitals with state-level comparisons.

**[healthcare-access-risk-analysis](https://github.com/ksolano220/healthcare-access-risk-analysis)** · [live map](https://ksolano220.github.io/healthcare-access-risk-analysis/)
County-level risk scoring for 3,200+ US counties using uninsured population data and hospital density. Interactive Folium choropleth for resource planning.

**[clinical-trial-trends](https://github.com/ksolano220/clinical-trial-trends)**
Exploratory analysis of 10,000 ClinicalTrials.gov trials. Sponsor patterns, phase completion rates, and geographic distribution.

### Systems & Automation

**[autonomous-claims-workflow](https://github.com/ksolano220/autonomous-claims-workflow)**
Multi-agent public-benefits workflow on IBM watsonx.ai + Granite, built as a solo submission to the IBM SkillsBuild AI Experiential Learning Lab. Intentionally designed to produce unsafe action proposals so that [Sentra](https://github.com/ksolano220/sentra) can intercept them.

## Skills

- **Data:** SQL, Python (pandas, NumPy), data modeling, ETL
- **Analysis:** exploratory analysis, cohort analysis, A/B testing, risk scoring
- **Visualization:** Streamlit, Plotly, matplotlib, Folium, Tableau
- **Applied AI:** LoRA / QLoRA fine-tuning, Hugging Face Transformers, PyTorch, multi-agent systems, IBM watsonx.ai / Granite
- **Backend:** Node.js, Express, MongoDB, Firebase, FastAPI
- **Product:** iOS, React Native, user research, design systems

## Activity

![Katherine's GitHub stats](https://github-readme-stats.vercel.app/api?username=ksolano220&show_icons=true&count_private=true&hide_border=true)
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=ksolano220&layout=compact&hide_border=true&langs_count=8)

## Contact

- Email: [solanokatherine220@gmail.com](mailto:solanokatherine220@gmail.com)
- LinkedIn: [linkedin.com/in/katherinesolano](https://www.linkedin.com/in/katherinesolano)
- New York, NY
