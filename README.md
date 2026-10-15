<img src="assets/banner.png" alt="Hey, I'm Aryan. Building the infrastructure that runs AI agents." width="100%" />

<h2>Hey, I'm Aryan 👋</h2>

Student developer from Bengaluru, **building the infrastructure that runs AI agents.**
I work on the unglamorous parts: backends, eval harnesses, monitoring and deployment, the stuff that keeps agents and ML models honest in production.

`Backend` · `MLOps` · `Agentic AI`

### Toolkit

| | |
|:--|:--|
| **stack** | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![Node.js](https://img.shields.io/badge/Node.js-5FA04E?style=flat-square&logo=nodedotjs&logoColor=white) ![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=flat-square&logo=supabase&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) |
| **cloud** | ![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white) ![EC2](https://img.shields.io/badge/EC2-FF9900?style=flat-square&logo=amazonec2&logoColor=white) ![S3](https://img.shields.io/badge/S3-569A31?style=flat-square&logo=amazons3&logoColor=white) ![Lambda](https://img.shields.io/badge/Lambda-FF9900?style=flat-square&logo=awslambda&logoColor=white) |
| **agents** | ![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white) ![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat-square&logo=ollama&logoColor=white) ![Anthropic](https://img.shields.io/badge/Anthropic_SDK-191919?style=flat-square&logo=anthropic&logoColor=white) |
| **devops** | ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white) ![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=jenkins&logoColor=white) ![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black) ![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white) |
| **ml** | ![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white) ![Hugging Face](https://img.shields.io/badge/Hugging_Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black) |

### What I'm building

**[RegressionGate](https://github.com/risaryan9/regressiongate)**: CI eval and tracing harness for tool-using LLM agents. Every prompt or model change replays a versioned dataset through deterministic checks (tool calls, actions, cost, latency) and then a cached LLM-as-judge. Pass-rate regressions fail a required GitHub Actions check and block the merge, and every run is stored as a span tree of LLM and tool calls, so a failing case traces back to the exact step that broke.
`Python` `Claude` `LLM-as-judge` `Tracing` `GitHub Actions`

**[Plainsight](https://github.com/risaryan9/plainsight)** *(in progress)*: agentic APK threat-analysis pipeline. Androguard static analysis (APKs are never executed) runs in a containerised AWS Lambda worker. ML anomaly scores with SHAP explanations feed a LangGraph multi-agent system on Claude, which checks the app's permissions and behaviour against what it claims to do. The scores are computed in code, and the LLM only explains them.
`Python` `LangGraph` `Claude` `AWS Lambda` `S3` `FastAPI`

**[Seraph](https://github.com/risaryan9/project-seraph)**: distributed telemetry pipeline for concurrent ML workloads, with phase-level attribution (train / infer / data). Instrumented jobs publish 13 resource metrics to partitioned Kafka topics. Consumer groups batch-write them (50 samples / 500 ms) to InfluxDB, tagged by model and phase, and FastAPI serves them over REST and WebSocket to an [observability console](https://github.com/risaryan9/project-seraph-frontend).
`Python` `Kafka` `InfluxDB` `FastAPI` `Docker`

### Stats

<p>
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=risaryan9&show_icons=true&hide_border=true&theme=transparent&hide_rank=true" alt="GitHub stats" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=risaryan9&layout=compact&hide_border=true&theme=transparent&langs_count=6" alt="Top languages" />
</p>
<p>
  <img src="https://streak-stats.demolab.com/?user=risaryan9&hide_border=true&theme=transparent" alt="GitHub streak" />
</p>
