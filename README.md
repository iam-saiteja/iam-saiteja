<div align="center">

# Thanniru Sai Teja

### AI Systems Researcher · Building memory, attention and inference systems from first principles

[![Typing SVG](https://readme-typing-svg.demolab.com/?lines=Independent+AI+Researcher;Attention-Free+%26+Memory+Architectures;Consumer+Hardware+Inference+Engineering;AI-Native+OS+in+Rust+%28NOUS%29;B.Tech+CS+%28Data+Science%29+%40+BVRIT&font=Fira+Code&center=true&width=580&height=45&color=58A6FF&vCenter=true&size=22&pause=1500)](https://git.io/typing-svg)

[![Portfolio](https://img.shields.io/badge/-Portfolio-000000?style=flat-square&logo=vercel&logoColor=white)](https://thannirusaiteja.me)
[![LinkedIn](https://img.shields.io/badge/-LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/thannirusaiteja)
[![Email](https://img.shields.io/badge/-Email-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:iamsaitejathanniru@gmail.com)

</div>

---

## About Me

I'm a B.Tech Computer Science (Data Science) student at **BVRIT Hyderabad**, currently working as **Tech Lead at Stud Entertainments**, with prior internship experience at **AWS, IBM, and Google**. Outside of coursework and internships, I run an independent research track focused on making large-model architectures -- attention, memory, inference -- work under real hardware constraints instead of just on paper.

Most of what is here falls into four buckets:

- **Memory and attention architectures** for foundation models -- designing systems that scale sub-quadratically without giving up retrieval quality
- **Consumer-hardware inference engineering** -- squeezing large-model workloads onto a single 4GB-VRAM GPU through quantization, caching, and prediction tricks
- **AI-native systems** -- building operating system substrates where the AI model is the kernel, not an application running on top of one
- **Developer tooling** -- small, sharp tools (compilers, package managers, UI libraries) that solve one problem cleanly

I evaluate my own work adversarially before anyone else gets to. If a result looks too good, I go find out why before I publish it.

---

## Featured Work

### Research and Model Architecture

<table>
<tr>
<td width="50%">

**[HGDM -- Hierarchical Gated Delta Memory](https://github.com/iam-saiteja/HGDM-Hierarchical-Gated-Delta-Memory)**

100% attention-free, byte-level sequence architecture with Hierarchical Temporal Decimation, Factored Bilinear State Highways, and a custom Triton fused scan engine (Nitro). Trained at 1B parameters on 1.46B tokens. Achieves O(1) inference memory -- VRAM footprint stays constant regardless of context length, verified empirically across 20x prompt scaling.

`Python` `Triton` `CUDA`

</td>
<td width="50%">

**[NCM -- Native Cognitive Memory](https://github.com/iam-saiteja/NCM)**

Tensor-based episodic memory with state-conditioned retrieval for AI systems. Uses a four-field distance function -- semantic, emotional, state-conditioned, and temporal -- as the native memory subsystem for agent-style architectures. Ported to `no_std` Rust as the memory core of NOUS.

`Python` `Rust`

</td>
</tr>
</table>

**Active research (not yet public):**

- **ZS-ISAB** -- a method for scaling TabPFN's attention from quadratic to linear complexity via seeded anchor selection, an online softmax accumulator, and a zero-shot attention mask -- enabling 500K+ row inference on 4GB VRAM. Currently in iteration toward TMLR submission.
- **PAS-Offload** -- a consumer-GPU LLM inference engine combining CPU-side low-rank activation prediction, transposed column-major weight caching, and dynamic 2-bit weight slicing, benchmarked on an RTX 3050.

---

### Systems

<table>
<tr>
<td width="50%">

**[NOUS -- Cognitive Operating System](https://github.com/iam-saiteja/nuos)**

A bare-metal AI-native OS in Rust for `x86_64`. Memory is addressed by semantic embeddings rather than numerical pointers. The resident kernel is not a scheduler for programs -- it is a five-level HTSPC-ED recurrent neural model with NCM integration, event-driven gating, and Hebbian plastic weight updates. Ships a real-time UEFI framebuffer dashboard and a capability-gated intent syscall interface.

`Rust` `x86_64` `UEFI` `no_std`

</td>
<td width="50%">

**[AXIS](https://github.com/iam-saiteja/AXIS)**

A small, rule-based, deterministic compiler that takes a plain app description and generates native Web, Android, and iOS UI code without an LLM in the loop.

`TypeScript`

**[PyLite-Manager](https://github.com/iam-saiteja/PyLite-Manager)**

A Tkinter GUI for managing Python virtual environments and pip packages -- for when you do not want to remember venv flags.

`Python`

</td>
</tr>
</table>

---

### Applied and Shipped

<table>
<tr>
<td width="50%">

**[FormatForge](https://github.com/iam-saiteja/FormatForge)** -- [Live demo](https://formatforge.streamlit.app/)

Streamlit app powered by Gemini 2.5 Flash Image that turns one uploaded photo into platform-ready assets for Amazon, Flipkart, Instagram, Spotify, and more -- with in-place AI re-editing via chat instructions.

`Python` `Streamlit` `Gemini` -- 1 star, 2 forks

</td>
<td width="50%">

**[react-scroll-media](https://github.com/iam-saiteja/react-scroll-media)**

Lightweight React library for cinematic scroll-driven image sequences -- eager/lazy frame loading, TypeScript support, SSR-safe, and built-in accessibility (respects `prefers-reduced-motion`).

`TypeScript`

</td>
</tr>
</table>

<details>
<summary><strong>Other repositories</strong></summary>
<br>

- **[Windows-MCP](https://github.com/iam-saiteja/Windows-MCP)** -- contributing to an MCP server for computer-use automation on Windows
- **[ailang-py](https://github.com/iam-saiteja/ailang-py)** -- Python project for AI-native language utilities
- **[VoxMimic](https://github.com/iam-saiteja/VoxMimic)** -- voice cloning and mimicry system
- **[storyboarding](https://github.com/iam-saiteja/storyboarding)** -- AI-assisted storyboard generation
- **[synthetic-life-system](https://github.com/iam-saiteja/synthetic-life-system)** -- emergent behavior and synthetic agent simulation
- **[Event-Ticket-Booking-System](https://github.com/iam-saiteja/Event-Ticket-Booking-System)**, **[Buzzer](https://github.com/iam-saiteja/Buzzer)**, **[SmartFarm](https://github.com/iam-saiteja/SmartFarm)**, **[Chaff](https://github.com/iam-saiteja/Chaff)** -- earlier web and coursework projects

</details>

---

## Tech Stack

**Core**

![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/-PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![Rust](https://img.shields.io/badge/-Rust-000000?style=flat-square&logo=rust&logoColor=white)
![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![C++](https://img.shields.io/badge/-C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![CUDA](https://img.shields.io/badge/-CUDA-76B900?style=flat-square&logo=nvidia&logoColor=white)

**ML and Infra**

![Triton](https://img.shields.io/badge/-Triton-000000?style=flat-square)
![HuggingFace](https://img.shields.io/badge/-HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![Ollama](https://img.shields.io/badge/-Ollama-000000?style=flat-square)
![Streamlit](https://img.shields.io/badge/-Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![React](https://img.shields.io/badge/-React-61DAFB?style=flat-square&logo=react&logoColor=black)

**Cloud and Tools**

![AWS](https://img.shields.io/badge/-AWS-232F3E?style=flat-square&logo=amazon-aws&logoColor=white)
![GCP](https://img.shields.io/badge/-Google_Cloud-4285F4?style=flat-square&logo=google-cloud&logoColor=white)
![Git](https://img.shields.io/badge/-Git-F05032?style=flat-square&logo=git&logoColor=white)
![VS Code](https://img.shields.io/badge/-VS_Code-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white)

---

## GitHub Stats

<div align="center">

<img height="165" src="https://github-stats-extended.vercel.app/api?username=iam-saiteja&show_icons=true&theme=github_dark&hide_border=true&count_private=true" />
<img height="165" src="https://github-stats-extended.vercel.app/api/top-langs/?username=iam-saiteja&layout=compact&theme=github_dark&hide_border=true" />
<br>

<img src="https://github-readme-streak-stats.herokuapp.com/?user=iam-saiteja&theme=github-dark-blue&hide_border=true" />

</div>

---

## Currently

- Iterating on **ZS-ISAB** toward TMLR submission -- resolving TabICL baseline verification and regenerating figures against the current seeded-anchor architecture
- Running a 91-dataset **TabZilla benchmark** against tree-based baselines
- Prototyping row-ordering strategies for fusing **MiniMax Sparse Attention** into a TabPFN-style tabular foundation model
- Continuing development on **NOUS** -- next milestone is a persistent NVMe driver replacing the simulated cold storage tier
- Open to research collaborations on efficient attention, memory-augmented architectures, and consumer-hardware ML systems

---

<div align="center">
<i>Not currently obsessed with anything. Everything above is currently obsessing me.</i>
</div>
