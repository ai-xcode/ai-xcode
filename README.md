<h1 align="center">Sewa Singh Bajwa</h1>
<p align="center">
  <em>AI infrastructure &amp; agent autonomy</em>
</p>
<p align="center">
  <code>vLLM</code> · <code>NCCL</code> · <code>Blackwell</code> · <code>cognitive architectures</code> · <code>quant trading</code> · <code>quantum computing</code>
</p>

---

### Recent work

**[`vllm-blackwell-nvfp4`](https://github.com/ai-xcode/vllm-blackwell-nvfp4)** — NVFP4 conversion + serve workflow for RTX PRO 6000 Blackwell. Documents the `curand_kernel.h` workaround required to load NVFP4 models on default CUDA 13 installs (the `libcurand-dev-13-0` headers aren't pulled in by default; either apt-install them or use the pip-wheel header trick the launcher script bakes in). Ships a NiceGUI dashboard that wraps convert / serve / bench with click-to-run forms, and a `bench_tps.py` harness usable against any OpenAI-compatible endpoint.

> **10-run single-stream throughput** (stdev < 0.1 tok/s on all three): Qwen3-4B-NVFP4 **213.6 tok/s** · Qwen3-14B-NVFP4 **100.9 tok/s** · DeepSeek-R1-Distill-14B-NVFP4 **96.8 tok/s**. Honest list of architectures that don't yet convert cleanly (Qwen3-Next, Qwen3.5 vision MoEs, Qwen2.5-VL). MIT licensed.

---

**[`vllm-blackwell-tp2-fix`](https://github.com/ai-xcode/vllm-blackwell-tp2-fix)** — Diagnosed and worked around two distinct deadlocks during vLLM tensor-parallel startup on dual RTX PRO 6000 Blackwell (PCIe-only, no NVLink). Tracks upstream [`vllm-project/vllm#33041`](https://github.com/vllm-project/vllm/issues/33041), which has no in-tree fix.

> **174 tok/s** on Qwen3-Coder-80B with TP=2 restored via two flags. Includes 4-config benchmark (INT4/FP8 × TP=1/TP=2) and 150–600 W power-curve sweep (300 W = perf/watt sweet spot). MIT licensed.

---

### Domains

- **AI infrastructure** — local LLM inference at scale: vLLM internals, NCCL transport, CUDA 13, multi-tier model orchestration on Blackwell.
- **Agent autonomy** — long-horizon planning, tool-use chains, self-modeling, and metacognition for assistants that don't lose state across sessions.
- **Cognitive architectures** — memory + perception + reasoning systems that extend a base LLM into something more agent-like and persistent.
- **Quantitative trading** — automated strategies, backtesting, broker integration, risk control.
- **Quantum computing** — exploring near-term applications and hybrid classical/quantum workflows.

---

### Currently exploring

- NVFP4 quantization conversions for the 100–340 B parameter range — what fits 192 GB and at what quality cost.
- Multi-model coordination on shared GPU memory with hot-swap eviction.
- Practical agent self-evaluation loops (the kind that survive past 50 turns).

---

### Reach me

- **LinkedIn** — [add your LinkedIn URL here]
- **GitHub** — [@ai-xcode](https://github.com/ai-xcode)
- **Email** — `205054636+ai-xcode@users.noreply.github.com` (private noreply)

> Open to: **AI infrastructure**, **inference engineering**, **applied agent research**, **GPU systems** roles. Remote or on-site.

---

<sub>Last updated 2026-05-03. Source: <a href="https://github.com/ai-xcode/ai-xcode">github.com/ai-xcode/ai-xcode</a></sub>
