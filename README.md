<div align="center">

# Hi, I'm Hamza Usta 👋

### ML Systems · Compiler Infrastructure · HPC · AI Agents

<p>
  Computer Engineering student at Istanbul University.<br>
  Building native, performance-oriented systems at the intersection of
  machine learning, compilers, heterogeneous computing and AI agent infrastructure.
</p>

<p>
  <a href="https://github.com/onlyxItachi/GAFIME">
    <img src="https://img.shields.io/badge/GAFIME-Feature%20Interaction%20Engine-blue?style=for-the-badge&logo=github" />
  </a>
  <a href="https://github.com/onlyxItachi/PerfDigest-MCP">
    <img src="https://img.shields.io/badge/PerfDigest-MCP%20Profiler%20Bridge-green?style=for-the-badge&logo=github" />
  </a>
</p>

<p>
  <img src="https://komarev.com/ghpvc/?username=onlyxItachi&style=flat-square&label=Profile+Views" />
  <img src="https://img.shields.io/github/followers/onlyxItachi?style=flat-square&label=Followers" />
</p>

</div>

---

## 🧭 What I Build

I am interested in the layers where machine-learning ideas stop being
notebooks and become real systems:

- ⚙️ Native execution engines
- 🧠 Machine-learning systems and feature discovery
- 🧩 Compilers, DSLs and intermediate representations
- 🚀 CPU, GPU and heterogeneous computing
- 🤖 AI coding-agent infrastructure
- 📊 Deterministic benchmarking and performance analysis
- 🔬 Research-driven engineering

My work usually starts with a question like:

> Can this abstraction be made faster, more deterministic, more inspectable,
> or closer to the hardware?

And then it somehow turns into a C++, Rust, CUDA, ROCm or compiler project. 😅

---

<div align="center">

## 🧮 Engineering Philosophy

$$
\boxed{
\text{Useful AI Systems}
=
\text{Algorithms}
\times
\text{Systems}
\times
\text{Evidence}
}
$$

$$
\text{Performance}
\neq
\text{Guesswork}
$$

$$
\text{Correctness}
+
\text{Measurement}
+
\text{Reproducibility}
\longrightarrow
\text{Shippable Engineering}
$$

</div>

I care about systems whose claims can be supported by:

- reproducible experiments,
- benchmarks,
- profiler reports,
- regression tests,
- explicit acceptance criteria,
- and inspectable artifacts.

A confident answer is useful.

A verified answer is better.

---

# 🚀 Featured Projects

## ⚡ GAFIME

### GPU-Accelerated Feature Interaction Mining Engine

[![Repository](https://img.shields.io/badge/Repository-GAFIME-blue?style=flat-square&logo=github)](https://github.com/onlyxItachi/GAFIME)
[![PyPI](https://img.shields.io/pypi/v/gafime?style=flat-square&logo=pypi)](https://pypi.org/project/gafime/)
[![License](https://img.shields.io/github/license/onlyxItachi/GAFIME?style=flat-square)](https://github.com/onlyxItachi/GAFIME/blob/main/LICENSE)

GAFIME is a native feature-interaction mining engine for tabular,
structured and time-series machine-learning workflows.

It is designed for workloads where interaction candidates, threshold regions
and temporal transformations become too expensive to explore through ordinary
Python loops or repeated model training.

```text
Python API
    │
    ├── C++ native core
    ├── Rust scheduling and orchestration
    ├── CUDA backend
    ├── ROCm / HIP backend
    └── Apple Metal backend
```

### GAFIME currently explores

- continuous feature interactions,
- soft discrete thresholds and intervals,
- rectangular decision regions,
- causal time-series transformations,
- native CPU SIMD execution,
- GPU-accelerated candidate evaluation,
- scikit-learn integration,
- large-file streaming workflows,
- and future compiler-driven execution.

The larger goal is not merely to generate more features.

It is to build an engine capable of discovering, evaluating and executing
useful feature structures efficiently across different hardware backends.

<div align="center">

$$
\text{Feature Search Cost}
\propto
\binom{d}{k}
\times
N
\times
C_{\text{candidate}}
$$

$$
\text{GAFIME}
\Longrightarrow
\text{Native Search}
+
\text{Hardware-Aware Execution}
+
\text{Structured Reports}
$$

</div>

---

## 📉 PerfDigest MCP

### Token-Efficient Performance Intelligence for LLM Coding Agents

[![Repository](https://img.shields.io/badge/Repository-PerfDigest--MCP-green?style=flat-square&logo=github)](https://github.com/onlyxItachi/PerfDigest-MCP)
[![License](https://img.shields.io/badge/License-Apache--2.0-green?style=flat-square)](https://github.com/onlyxItachi/PerfDigest-MCP/blob/main/LICENSE)

PerfDigest is a local MCP server that sits between performance profilers
and AI coding agents.

Profiler reports are often enormous, vendor-specific and extremely expensive
to place directly inside an LLM context window.

PerfDigest turns those reports into compact, deterministic and numeric digests
while preserving references to the original data.

```text
Profiler Output
      │
      ▼
┌─────────────────┐
│   PerfDigest    │
│ Parse · Normalize│
│ Route · Compress │
└─────────────────┘
      │
      ▼
Compact metrics for coding agents
```

### Supported performance domains

| Backend | Domain | Typical tools |
|---|---|---|
| NVIDIA | GPU kernels | Nsight Compute |
| AMD | GPU kernels | rocprof |
| Linux | CPU functions | perf |
| Apple | GPU passes | Metal / xctrace |

One of the project's most important rules is:

$$
\texttt{None} \neq 0
$$

A missing metric must never silently become a zero.

Because feeding fabricated performance information to an AI agent is worse
than returning no information at all.

PerfDigest is intentionally a translator and router, not an oracle.

It exposes evidence efficiently.

The model still has to reason about that evidence.

---

## 🧠 Synclave

### Local-First Multi-Agent Engineering Runtime

> 🚧 In active development — planned for a future public release.

Synclave is an upcoming Git-native, event-sourced execution runtime for
coordinating heterogeneous AI coding agents.

Instead of merging every model into a single synthetic assistant,
Synclave keeps agents independent.

Different agents may:

- propose competing plans,
- claim engineering tasks,
- challenge technical decisions,
- exchange evidence,
- run experiments,
- review commits,
- and verify explicit acceptance criteria.

```text
Human Intent
     │
     ▼
Independent Coding Agents
     │
     ├── Claims
     ├── Challenges
     ├── Evidence
     ├── Experiments
     └── Reviews
     │
     ▼
Verified Artifacts and Shippable Work
```

The core idea is simple:

<div align="center">

$$
\text{Agent Confidence}
<
\text{Reproducible Evidence}
$$

$$
\text{Chat History}
\neq
\text{Durable System State}
$$

$$
\text{Done}
\iff
\text{Acceptance Criteria Satisfied}
$$

</div>

Synclave is being designed around:

- Rust-based local runtime infrastructure,
- typed event protocols,
- SQLite-backed durable state,
- isolated Git worktrees,
- artifact and benchmark exchange,
- crash-safe replay,
- policy and approval boundaries,
- independent agent review,
- and provider-independent integrations.

The intended outcome is not another chatbot router.

It is execution infrastructure for agents that must cooperate,
disagree, verify and ship.

---

# 🛤️ How I Got Here

My GitHub history reflects a gradual descent through the software stack.

```text
C / C++ and OOP projects
          │
          ▼
Game systems and Vulkan experiments
          │
          ▼
DSL and compiler architecture
          │
          ▼
Native ML and feature-engineering runtimes
          │
          ▼
CUDA · ROCm · Metal · SIMD
          │
          ▼
LLM tooling and performance infrastructure
          │
          ▼
Multi-agent execution systems
```

I began with game and object-oriented programming projects,
including experiments around intelligent NPC systems and a minimal
Vulkan-based engine core.

That eventually led me toward questions about:

- code generation,
- compiler architecture,
- intermediate representations,
- runtime specialization,
- kernel execution,
- hardware-aware optimization,
- and deterministic AI-assisted engineering.

Today, most of my projects live somewhere between machine learning
and systems programming.

---

# 🔬 Research Interests

## Tabular Deep Learning

I am researching how neural networks can discover and integrate the kinds of
axis-aligned structures that gradient-boosted trees naturally exploit.

This includes:

- residual-directed feature mining,
- differentiable decision paths,
- learnable threshold structures,
- gated feature augmentation,
- causal time-series transformations,
- and hardware-accelerated candidate search.

<div align="center">

$$
r_i = y_i - \hat{y}_i
$$

$$
\text{Next Feature}
=
\arg\max_{\phi}
\operatorname{Score}\left(\phi(X), r\right)
$$

$$
\phi_{\text{path}}(x)
=
\prod_{k=1}^{m}
\sigma
\left(
s_k \cdot d_k \cdot (x_{f_k}-t_k)
\right)
$$

</div>

The broader question is:

> Can a neural network learn the representation it is missing,
> instead of only scaling its parameter count?

---

## Compiler-Driven Machine Learning

I am also interested in execution systems where models, transformations
and hardware kernels are optimized as a unified program.

Potential directions include:

- operation fusion,
- model-specific code generation,
- execution graph specialization,
- static interaction planning,
- runtime backend selection,
- kernel caching,
- and hardware-specific compilation.

<div align="center">

$$
\text{Model}
+
\text{Execution Graph}
+
\text{Target Hardware}
\longrightarrow
\text{Specialized Program}
$$

</div>

---

## AI Agent Infrastructure

Coding agents are becoming capable enough that their biggest limitations
are increasingly infrastructural:

- context loss,
- weak state management,
- unverifiable claims,
- shared-workspace conflicts,
- missing provenance,
- and ambiguous completion conditions.

I am interested in systems where agents operate through durable state,
typed protocols, isolated workspaces and measurable acceptance contracts.

---

# 🧰 Technologies

## Languages

<p>
  <img src="https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white" />
  <img src="https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white" />
  <img src="https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
</p>

## Compute and Systems

<p>
  <img src="https://img.shields.io/badge/CUDA-76B900?style=for-the-badge&logo=nvidia&logoColor=white" />
  <img src="https://img.shields.io/badge/ROCm-ED1C24?style=for-the-badge&logo=amd&logoColor=white" />
  <img src="https://img.shields.io/badge/Metal-000000?style=for-the-badge&logo=apple&logoColor=white" />
  <img src="https://img.shields.io/badge/OpenMP-0095D5?style=for-the-badge" />
  <img src="https://img.shields.io/badge/SIMD-AVX2%20%7C%20AVX--512-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Vulkan-AC162C?style=for-the-badge&logo=vulkan&logoColor=white" />
</p>

## Machine Learning and Data

<p>
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" />
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white" />
  <img src="https://img.shields.io/badge/Polars-CD792C?style=for-the-badge&logo=polars&logoColor=white" />
  <img src="https://img.shields.io/badge/LightGBM-02569B?style=for-the-badge" />
</p>

## Tooling and Infrastructure

<p>
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" />
  <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white" />
  <img src="https://img.shields.io/badge/CMake-064F8C?style=for-the-badge&logo=cmake&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" />
  <img src="https://img.shields.io/badge/MCP-Protocol-purple?style=for-the-badge" />
</p>

---

# 🎯 Current Focus

```yaml
current_projects:
  - GAFIME v0.5.x architecture
  - native CPU and GPU execution
  - compiler-oriented feature pipelines
  - tabular deep-learning research
  - Synclave agent runtime
  - token-efficient performance tooling

learning:
  - compiler internals
  - LLVM architecture
  - GPU kernel optimization
  - heterogeneous runtime design
  - distributed and event-sourced systems

long_term_goal:
  - build intelligent systems that are fast,
    measurable, reproducible and close to the hardware
```

---

# 📊 GitHub Activity

<div align="center">

<img
  height="170"
  src="https://github-readme-stats.vercel.app/api?username=onlyxItachi&show_icons=true&hide_border=true&include_all_commits=true&count_private=true"
/>

<img
  height="170"
  src="https://github-readme-stats.vercel.app/api/top-langs/?username=onlyxItachi&layout=compact&hide_border=true&langs_count=8"
/>

</div>

<div align="center">

<img
  src="https://github-readme-streak-stats.herokuapp.com/?user=onlyxItachi&hide_border=true"
/>

</div>

---

# 🤝 Collaboration

I am especially interested in collaborating on projects involving:

- native machine-learning infrastructure,
- compiler and runtime engineering,
- GPU and heterogeneous computing,
- tabular deep learning,
- performance-analysis tooling,
- AI coding agents,
- MCP infrastructure,
- and research-oriented open-source systems.

---

<div align="center">

## Final Principle

$$
\boxed{
\text{Build deeply. Measure honestly. Ship reproducibly.}
}
$$

### Thanks for visiting 👋

<a href="mailto:hamzausta2222@gmail.com">
  <img src="https://img.shields.io/badge/Email-hamzausta2222%40gmail.com-red?style=for-the-badge&logo=gmail&logoColor=white" />
</a>

<a href="https://github.com/onlyxItachi">
  <img src="https://img.shields.io/badge/GitHub-onlyxItachi-black?style=for-the-badge&logo=github" />
</a>

</div>
