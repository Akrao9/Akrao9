### Hi, I'm Ankamma Rao — I build generative AI and ML systems, from research to production.

Software Engineer (AI/ML) at **Resonate Technologies**, working on RAG and self-correcting LLM pipelines for medical coding. Previously backend/ML at Digital Factory Inc. MS in Computer Science from NJIT.

- 🔭 Currently training **Linarix**, a ~900M-parameter hybrid-attention text-to-image diffusion model — [try it on Hugging Face](https://huggingface.co/spaces/akrao9/Linarix-v2-T2I)
- 🛠️ I ship upstream fixes to real ML infra — merged PRs in [`Lightning-AI/pytorch-lightning`](https://github.com/Lightning-AI/pytorch-lightning) (31k★) and [`fla-org/flash-linear-attention`](https://github.com/fla-org/flash-linear-attention) (5.6k★)
- 🧠 Focus areas: diffusion models, flow matching, linear attention, multimodal learning, RAG
- 📫 Reach me: [LinkedIn](https://www.linkedin.com/in/ankamma-rao-bandi-35ab7616b/) · [Hugging Face](https://huggingface.co/akrao9) · ak.rao.bandi2@gmail.com

---

#### Open Source Contributions

**[flash-linear-attention](https://github.com/fla-org/flash-linear-attention)** — extended backend dispatch for a fused TileLang kernel (FlashQLA) to support NVIDIA SM120 (Blackwell) GPUs, which previously fell back to a slower Triton path. Added grad-state-aware routing and parametrized parity tests. Validated on physical RTX PRO 6000 Blackwell hardware: within 0.6% parity of reference, up to 2.6x forward-pass speedup over Triton across sequence lengths to 32K tokens.

**[pytorch-lightning](https://github.com/Lightning-AI/pytorch-lightning)** — diagnosed and fixed a training UX bug where progress bars/ETAs were wrong for iterable datasets + `max_steps` + gradient accumulation. Root-caused a unit mismatch between optimizer steps and batch-level updates, added regression tests, and landed the fix upstream.

#### Research Projects

| Project | Description |
|---|---|
| [Linarix](https://huggingface.co/spaces/akrao9/Linarix-v2-T2I) | ~900M-param hybrid GDN2/softmax-attention flow-matching text-to-image model, Qwen3.5-4B conditioning, near-flat inference memory scaling to batch 90 |
| [VGGT-LACT](https://github.com/Akrao9/VGGT-LACT) | Linear-memory 3D scene reconstruction — replaces quadratic attention in VGGT with LaCT-style fast-weight GLU blocks; 2.1x throughput, 59% less VRAM |
| [MidMamba](https://github.com/Akrao9/MidMamba-Optimal-Execution) | PPO + Mamba-2 encoder for optimal trade execution on L2 order-book data, benchmarked against TWAP/Almgren-Chriss |

#### Stack

`Python` `PyTorch` `JAX` `Hugging Face` `CUDA/Triton` `AWS (SageMaker, Lambda)` `Docker` `Kubernetes` `FastAPI` `PostgreSQL`

---

![GitHub stats](https://github-readme-stats.vercel.app/api?username=Akrao9&show_icons=true&theme=default&hide_title=true&hide_border=true)
