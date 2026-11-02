# Hi, I'm Ankamma Rao Bandi

Machine Learning Engineer focused on diffusion models, linear attention, and efficient training and inference. I build generative models and production LLM systems, and contribute fixes to open-source ML infrastructure.

MS in Computer Science from New Jersey Institute of Technology.

## Featured project: Linarix

**[Linarix](https://github.com/Akrao9/Linarix-Text-to-Image-Hybrid-Attention-Diffusion-Model)** is a text-to-image flow-matching model with an approximately **890M-parameter denoiser**, a GatedDeltaNet-2 condition encoder, a full-attention DDT decoder, and frozen Qwen3.5-4B text conditioning.

- Built the model and training pipeline in PyTorch, with distributed training and memory-efficient optimization.
- Supports **1024 x 1024 generation**, STORK sampling, batched inference, and VAE slicing.
- Published model weights and an interactive Hugging Face demo.

[Code](https://github.com/Akrao9/Linarix-Text-to-Image-Hybrid-Attention-Diffusion-Model) · [Model weights](https://huggingface.co/akrao9/Linarix-v2) · [Try the demo](https://huggingface.co/spaces/akrao9/Linarix-v2-T2I) · [Training details](https://github.com/Akrao9/Linarix-Text-to-Image-Hybrid-Attention-Diffusion-Model/blob/main/docs/training.md)

## Open-source contributions

### Flash Linear Attention - merged

Enabled FlashQLA BF16 forward dispatch on **NVIDIA SM120 Blackwell GPUs**, with gradient-state safeguards, dtype checks, and parity tests. Benchmarks on an RTX PRO 6000 Blackwell measured up to **2.62x forward-pass speedup over the Triton backend** for the tested GatedDeltaNet operator configurations.

[PR #1094](https://github.com/fla-org/flash-linear-attention/pull/1094) · [Follow-up: exact SM120 capability matching, PR #1098](https://github.com/fla-org/flash-linear-attention/pull/1098)

### PyTorch Lightning - submitted

Diagnosed an optimizer-step versus batch-count mismatch that produced incorrect progress-bar totals and ETAs for iterable datasets with `max_steps` and gradient accumulation. Submitted a fix with parametrized regression tests.

[PR #21802](https://github.com/Lightning-AI/pytorch-lightning/pull/21802)

## LLM systems

I work on self-hosted LLM services, structured document extraction, RAG, model evaluation, and production monitoring. My serving experience includes **SGLang and vLLM**, continuous batching, prefix caching, and GPU memory tuning.

## Technical stack

| Area | Tools and techniques |
| --- | --- |
| Models and training | Python, PyTorch, FSDP, BF16, torch.compile, gradient checkpointing, Hugging Face Transformers, Diffusers |
| Inference and GPU optimization | SGLang, vLLM, Flash Linear Attention, TileLang, batched inference, KV caching |
| Production and MLOps | FastAPI, Docker, Kubernetes, AWS, MLflow, Weights & Biases, pytest, CI/CD |

## Connect

[LinkedIn](https://www.linkedin.com/in/ankamma-rao-bandi-35ab7616b/) · [Hugging Face](https://huggingface.co/akrao9) · [Email](mailto:akraobandi98@gmail.com)

