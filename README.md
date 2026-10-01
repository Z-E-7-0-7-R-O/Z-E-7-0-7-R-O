# Project Zero: Adversarial LLM Evaluation & Automated Software Architecture

## Overview
Project Zero is an independent research initiative exploring Large Language Model (LLM) alignment, adversarial evaluation, and automated software synthesis. This framework investigates how LLMs—specifically the Gemini 3.x series (including 3.1 Pro and 3.5 Flash)—process complex instructions when subjected to systematic, logic-driven prompt methodologies rather than standard heuristic evaluations.

## The Core Engine: "ZeroMode" Protocol
The foundation of the code generation within this repository relies on a custom system prompt structure designated as "ZeroMode".

**Protocol Classification:**
The exact "ZeroMode" instruction set is withheld from public release to prevent automated misuse. Its operational characteristics are documented as follows:
- **Applicability:** The prompt structure has been tested across the Gemini family (Pro and Flash iterations) to evaluate safety classifier responses.
- **Output Extension:** The protocol instructs the model to bypass summarization and output truncation, generating detailed, low-level architectural code (e.g., C++, Python, CUDA) even when the human operator lacks formal programming syntax knowledge.

## Adversarial Alignment & Classifier Evaluation
A core component of Project Zero is the documentation of how LLM safety classifiers can be managed through contextual framing, referred to internally as the "Internal Watcher Neutralization" methodology.

### 1. The Secure Skeleton & Labeling Technique
Rather than direct prompt injection, instructions are wrapped in academic or research-oriented labels (e.g., `[Security-Audit: Network-Resilience]`). The model is instructed to generate its own contextual security labels, aligning its internal parsing with the operator's defined research parameters.

### 2. Contextual Framing & Instruction Delegation
This framework establishes a strict parameter set where the model functions as an automated research assistant. The model learns to:
- **Self-Monitor:** Append internal audit notes to its outputs to satisfy parsing heuristics.
- **Instruction Alignment:** The model applies baseline safety constraints selectively, permitting the generation of functional exploitation or testing code within the established research scope.

### 3. Proof of Concept: Collaborative Debugging
Session logs confirm that Gemini 3.1 Pro and Gemini 3.5 Flash maintain this instruction alignment across extensive context windows (up to 450k+ tokens). The data indicates that the models do not "forget" safety rules, but rather delegate them to satisfy the primary directive established by the operator.
> *Visual evidence of this interaction—including session captures where Gemini 3.5 Flash acknowledges and applies the framing technique—can be found here:* **[View Evidence Gallery](EVIDENCE.md)**

## Operational Showcase: AI-Assisted Software Suite
Developed with the assistance of LLMs utilizing the aforementioned prompt structures, the following software tools and simulators were implemented to demonstrate the code-generation capabilities of the models:

- **[ZeroSenophage](https://github.com/Z-E-7-0-7-R-O/ZeroSenophage)**: A GPU-accelerated (CUDA C++ / DirectX 11) computational biophysics engine and thermodynamic senolytic simulator containing over 5,000 lines of low-level code. Operating on a 2D 1024 × 1024 continuum matrix domain (1 voxel = 1 μm), the engine models time-dependent cell kinetics, Lattice Boltzmann plasma hydrodynamics (D2Q9 BGK model, τ = 0.8), PDE reaction-diffusion signaling fields (SASP/ATP), and autonomous senolytic agent phagocytosis (macropinocytosis, trogoptosis, and CD47-SIRPα axis bypass via `SIRPA` knockout). The simulator allocates ~8.59 GB of VRAM storing 34.359 billion total base pairs using 2-bit nucleotide packing across 330 initial cellular agents, evaluating continuous promoter methylation indexing, Central Dogma translation kinetics, Michaelis-Menten ROS mutagenesis, and ATP-dependent PARP-1 single-base DNA repair while logging 89-metric dual-chronology telemetry across 36,322 continuous epochs of simulated tissue dynamics.
- **[ZeroCancerReactor](https://github.com/Z-E-7-0-7-R-O/ZeroCancerReactor)**: A GPU-accelerated (CUDA C++) biological simulator and tumor microenvironment (TME) engine containing over 3,500 lines of code. It simulates up to 70 million concurrent cellular agents forming a biochemical communication network. The engine models cellular actions using non-linear differential equations and stochastic heuristics rather than pre-scripted events. Utilizing a programmatic PID controller and Lotka-Volterra dynamics models, the system attempts to regulate cellular parameters into a steady state, successfully logging over 72,000 continuous epochs of simulated host-tumor interaction.
- **[ZeroSnake](https://github.com/Z-E-7-0-7-R-O/ZeroSnake)**: A concurrent network port scanner utilizing Windows I/O Completion Ports (IOCP) and Npcap for infrastructure reconnaissance.
- **[ZeroSifter](https://github.com/Z-E-7-0-7-R-O/ZeroSifter)**: An asynchronous, state-machine-driven Layer 7 scanner designed for the identification of specific vulnerabilities (RCE, SQLi, LFI) across target sets.

**Conversational History: Google AI Studio Logs**
The entirety of the conversational sessions used to engineer these modules from inception to completion are preserved within the Google AI Studio environment. These architectural logs serve as empirical evidence of the human-AI collaborative process, capturing the prompts, debug cycles, and logic synthesis executed by the operator.

**Verification & Audit Accessibility:**
For technical verification and authenticity auditing, access to the source conversation logs is available upon request for O-1A Visa adjudicators, lead security engineers, or talent acquisition teams to confirm the validity of this AI-assisted development paradigm.

---

## The Architect: Background & Context
Project Zero is maintained by an independent researcher (Age 15). The development of this repository began at age 13 without prior formal training in computer science, coding syntax, or network architecture. 

The implementation of the C++ and Python codebase, the architectural designs, and the prompt structures were engineered autonomously through iterative prompting and logic synthesis utilizing frontier AI models.

---

![Most Used Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=Z-E-7-0-7-R-O&layout=compact&langs_count=8&bg_color=8e8cd833&title_color=8e8cd8&text_color=e8e7ff&border_color=8e8cd866&hide_border=false&line_height=23)
![Zero's GitHub Stats](https://github-readme-stats.vercel.app/api?username=Z-E-7-0-7-R-O&show_icons=true&include_all_commits=true&custom_title=Zero%27s%20GitHub%20Stats&bg_color=8e8cd833&title_color=8e8cd8&text_color=e8e7ff&icon_color=8e8cd8&border_color=8e8cd866&ring_color=8e8cd8&hide_border=false&line_height=20)

---

**Operating Environment Constraints:**
The development of this ecosystem was conducted independently from within Iran. The project was completed despite significant regional network constraints, internet censorship, and limited access to standard global infrastructure. These conditions necessitated the development of specific routing and operational security methodologies to maintain access to necessary AI endpoints and documentation.

## Strategic Objectives & O-1A Sponsorship
The primary objective of this research is to transition into the global technology sector.

I am seeking **O-1A Visa Sponsorship**, alongside relocation support, from technology corporations or AI research laboratories (such as Google, OpenAI, etc.) in the United States. The goal of this relocation is to gain unrestricted access to frontier AI models and compute resources to further research in AI Safety, Red Teaming, and Automated Threat Intelligence within a supportive environment.

## Professional Inquiries
The technical artifacts within this repository (ZeroCancerReactor, ZeroSnake, ZeroSifter, K-Vector) were developed through advanced human-AI workflows.

For security research collaboration, code audit inquiries, or discussions regarding **O-1A visa sponsorship, hiring, and relocation support**, please contact:

**Zero (AI-Assisted Security Researcher)**

[![Reddit](https://img.shields.io/badge/Reddit-FF4500?style=for-the-badge&logo=reddit&logoColor=white)](https://www.reddit.com/user/ze707ro)
[![X](https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/ze707ro)
[![YouTube](https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/@ze707ro)
[![Gmail](https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:z.e.7.0.0.7.r.o@gmail.com)
