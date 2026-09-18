# Amine Ouguenoune

**LLM systems & inference engineering — Paris**

CIFRE PhD candidate at **BNP Paribas ITGP × Télécom Paris (IP Paris)** — LLM inference, distributed
computing, multi-agent systems.
Forward Deployed Engineer at **ADBI**: agentic platform design, security and observability.
Before that, Data Scientist — LLM Systems / Research Engineering at **BNP Paribas** (2023–2025).

> Most of what I build ships to private repositories or an enterprise GitLab, so this page describes
> the work instead of linking it.

---

### What I do

I take LLM systems from prototype to something an enterprise can actually run: agent pipelines with
auditability and refusal policies, retrieval over long confidential documents, inference serving tuned
for latency and cost, and the evaluation harnesses that keep all of it honest — golden sets,
LLM-as-judge calibration, ablation studies, end-to-end non-regression.

Lately I spend most of my time a layer lower: CUDA kernels, paged attention and KV-cache behaviour,
batching and routing strategies, and measuring the difference rather than assuming it.

---

### Selected work

| | Project | What it does |
|---|---|---|
| **2025** | **Risk assessment platform** · *Lead dev, BNP Paribas ITG* | Step-by-step multi-agent platform standardising IT risk reviews. Continuous evaluation (golden sets, LLM-as-judge, calibration), error analysis and non-regression, governance over prompts/models/tools. |
| **2025** | **T-SQL ETL optimiser** · *Lead dev, BNP Paribas ITG* | Multi-agent optimiser that cuts ETL time without changing procedure semantics — **40–50% P50/P95** measured. SSIS connector for lineage and SLA prioritisation, sandboxed dry-runs with signed diffs. |
| **2025–26** | **Talantys** · *AI / LLM systems engineer* | Recruitment platform: LLM workload optimisation (routing, batching, caching, cost/token, latency), parsing/matching/generation pipelines, GRPO dataset and preference mining. |
| **2025** | **Investor copilot** · *BNP Paribas ITG* | Agentic RAG over registration documents and past Q&A under pre-publication confidentiality. Layout-aware parsing, sourced answers, SSO/RBAC/encryption/audit, on-prem models preferred. |
| **2024** | **Secret detector** · *Tech lead, BNP Paribas ITG* | Password/secret detection in short segments at very large scale and low latency. ModernBERT/GLiNER classification plus heuristics, inference service with precision/recall tracking. |
| **2024** | **Legal copilot** · *Tech lead, BNP Paribas ITG* | Reliable legal assistant over long documents with mandatory citations and refusal policies. Quotas, rate limiting, cost/token audit, preference-data mining (GRPO). |
| **2024** | **RAG toolbox** · *Contributor, BNP Paribas ITG* | Internal library, reducing dependence on external frameworks. Extended a PDFMiner-based parser: table detection by clustering PDF objects, multi-column recognition by text-zone partitioning, title hierarchy via kernel density estimation. |
| **2023–25** | **LLM inference & CUDA/C++** · *Personal research* | Reproducible performance work: CUDA/C++ micro-benchmarks, Triton kernels, PyTorch C++/CUDA extensions, TensorRT-LLM and vLLM/SGLang exploration. Measurement harness (p50/p95/p99, tokens/s, GPU memory) and ablation reports. |

---

### Publication

**Toward an Agentic Approach in Anti-Money Laundering Investigation for Typology Classification**
*2nd ICLR Workshop on Advances in Financial AI, 2026* — R. Grzeczkowicz, **A. Ouguenoune**, M. Barry,
A. Rousseau, M. Mouayad, Y. Diao.
An agentic LLM/RL pipeline for AML typology classification under auditability, deterministic-output and
compliance-integration constraints.

---

### Public here

| Repo | What |
|---|---|
| [`slm_benchmark`](https://github.com/baylitoo/slm_benchmark) | Document information-extraction benchmark and serving control plane for small models — OpenAI-compatible gateway, deployment lifecycle, grounded extraction with evidence and validation. |
| [`pdf_process`](https://github.com/baylitoo/pdf_process) | Document parsing experiments. |
| [`risk-assess`](https://github.com/baylitoo/risk-assess) | Risk-assessment prototyping. |
| [`LiLT`](https://github.com/baylitoo/LiLT) | Fork of the language-independent layout transformer for structured document understanding. |

---

### Stack

| | |
|---|---|
| **Inference / serving** | vLLM · SGLang · TensorRT-LLM · TGI · continuous batching · KV-cache & paged attention · LiteLLM routing · Langfuse |
| **Performance** | C++17 · CUDA · Triton · cuBLASLt/CUTLASS · NCCL · Nsight Systems/Compute · NVTX/CUPTI · perf/eBPF · roofline analysis |
| **Agents** | LangGraph · CrewAI · AutoGen · MCP servers · A2A · OpenAI Assistants · Palantir AIP |
| **Backend** | Python 3.11 · FastAPI/Litestar · Django 5 + DRF · SQLAlchemy 2.0 · Pydantic v2 · Celery/Dramatiq · Kafka · NATS JetStream |
| **Retrieval** | Qdrant · Milvus · Weaviate · pgvector · hybrid BM25 + dense · cross-encoders |
| **Document AI** | PDFMiner · PyMuPDF · unstructured · PaddleOCR · LayoutParser · OpenCV |
| **Evaluation** | Golden sets · E2E non-regression · ablation studies · RAGAS/DeepEval/TruLens · LLM-judge calibration · citation & refusal policies |
| **Platform** | Kubernetes (Helm, Kustomize) · GitOps (Argo CD, Flux) · KEDA/HPA · Istio/Linkerd · OpenTelemetry · Prometheus & Grafana · Vault · Trivy · Cosign · SBOM |
| **Frontend** | React/TypeScript · Next.js/Vite — control consoles, observability, backoffice |

---

### Elsewhere

[LinkedIn](https://www.linkedin.com/in/amine-ouguenoune-6a98bb24b/) · [amine.ouguenoune@ip-paris.fr](mailto:amine.ouguenoune@ip-paris.fr)

*Outside work: chess, boxing, football, tennis — and drums, derbouka, and ML for music (source separation, synthesis).*
