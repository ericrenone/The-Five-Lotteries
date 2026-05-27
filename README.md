# The Five Lotteries

**Hardware-Software Co-Design Events That Locked In the Euclidean / Floating-Point / Matmul Stack — And the Geometric Reversal Forcing the Next $100B+ Infrastructure Cycle**

**Strategic Intelligence Report · 2027 Edition**  
**Infrastructure & Platforms · AI Systems Strategy**

**Prepared for:** Technology Executives · Infrastructure Investors · AI Architecture Leadership

**Primary Evidence Base:** 50+ peer-reviewed sources · NeurIPS 2025 · ICLR 2026 · Phys. Rev. E 2026 · IEEE TVLSI 2019 · arXiv preprints through Q2 2026

---

### The Bottom Line

Five independent hardware-software co-design decisions — made in **1985 (arithmetic)**, **1986 (optimization)**, **2017 (silicon)**, and now reaching ceilings in **biology compute (2028)** and **geometry (2025–2026)** — selected the representational substrate of every production AI system today.

These lotteries were not won on theoretical superiority. They were won on **perfect co-fitness** with the available hardware and software ecosystem (Hooker, *The Hardware Lottery*, CACM 2020, arXiv:2009.06489).

The compounding costs are now visible as three structural ceilings: iteration, curvature, and biology compute. The organizations that correctly identify which layer is failing, why it is failing, and what replaces it will capture the next infrastructure cycle. The ones that do not will fund it.

The **Representational Bundle Hypothesis (RBH, 2026)** provides the unified geometric picture of what the stack is actually computing. The 2023–2026 optimizer renaissance (Sophia, Muon, SOAP, FAdam) and the 2025–2026 CORDIC/hyperbolic breakthroughs mark the reversal.

**The co-design window is open (2026–2028).**

---

### Key Findings

| # | Finding | Strategic Urgency | Core Citation |
|---|---------|-------------------|---------------|
| 1 | Euclidean assumption structurally broken for hierarchical domains (negative Ricci curvature in token embeddings) | **Act Now** | Robinson et al. arXiv:2410.08993 (2024) & arXiv:2504.01002 (2025) |
| 2 | **Gradient Descent Lottery (1986)** discarded Fisher-Riemannian curvature, forcing 50–100× excess training steps | **Act Now** | Amari (1998); Liu et al. Sophia (2023) |
| 3 | Three ceilings (iteration, curvature, biology) now exceed replacement cost | **Act Now** | Geometry Report §2 |
| 4 | Grokking = holonomy accumulation in the representational bundle (capital allocation problem) | **Act Now** | Power et al. (2022); Xu Spectral Edge Thesis (2026); Muon acceleration (Tveit et al. 2025) |
| 5 | 2028 biology compute wall is architectural (pair-tensor / SE(3) / diffusion mismatches) | **Plan 2027** | Abramson et al. AlphaFold 3 (2024) |
| 6 | Lorentzian transition engineering obstacles cleared (HELM, Riemannian AdamW, CARMEN) | **Evaluate Now** | He et al. NeurIPS 2025 (arXiv:2505.24722) |
| 7 | **CORDIC (1959)** resurfaces as native substrate for iteration + hyperbolic ops (arithmetic lottery reversal) | **Invest Now** | Kumar et al. CARMEN arXiv:2605.06878 (2026); “CORDIC Is All You Need” arXiv:2503.11685 (2025) |
| 8 | Next moat is **geometric**, not scalar; co-design window open until incumbents ship extensions | **Invest Now** | Geometry Report §8–9 |

---

### Table of Contents

1. [The Five Lotteries — How the Stack Was Built](#1-the-five-lotteries)
2. [The Gradient Descent Lottery (1986) — The Pivotal Middle Layer](#2-the-gradient-descent-lottery)
3. [The Three Ceilings — Where the Stack Breaks](#3-the-three-ceilings)
4. [The Representational Bundle Hypothesis (RBH) — What the Stack Is Computing](#4-the-geometric-object)
5. [CORDIC Revival — Closing the Arithmetic Loop](#5-cordic-revival)
6. [The Lorentzian Transition — Market Sizing & Action Agenda](#6-the-lorentzian-transition)
7. [Ten Falsifiable Predictions](#7-predictions)
8. [Evidence Base & Sources](#evidence-base)

---

### 1. The Five Lotteries — How the Stack Was Built

**Lottery 1 — Arithmetic (1985)**  
IEEE 754 floating-point standardization won over fixed-point/CORDIC. Floating-point hides iteration count and bills in FLOPS; fixed-point exposes ticks and is natively iteration-friendly (Luo et al., IEEE TVLSI 2019). Energy overhead for iterative workloads: 2–10×.

**Lottery 2 — Optimization (1986)**  
Rumelhart, Hinton & Williams’ backpropagation + gradient descent paper committed the field to Euclidean parameter-space navigation (Nature 1986). Natural gradient descent (Amari 1998) was theoretically superior but O(N²) storage / O(N³) cost.

**Lottery 3 — Silicon (2017)**  
Vaswani et al. “Attention Is All You Need” (NeurIPS 2017, arXiv:1706.03762) was co-designed with Google TPU v2 systolic arrays (Jouppi et al. ISCA 2017). Every frontier model is now a Google-native workload running on Google-designed silicon.

**Lottery 4 — Biology Compute (ongoing → 2028 ceiling)**  
AlphaFold-class, RFdiffusion, Evo workloads require pair-tensor, SE(3) equivariance, diffusion denoising, Hyena filtering, and rank-one Sherman-Morrison updates — all emulated on GEMM at 3–12× overhead. Projected $490B annual structural waste by 2028.

**Lottery 5 — Geometry (2025–2026)**  
Token embedding spaces exhibit significantly negative Ricci curvature (Robinson et al. arXiv:2410.08993). Fully hyperbolic models now outperform Euclidean baselines (HELM, NeurIPS 2025).

---

### 2. The Gradient Descent Lottery (1986) — The Pivotal Middle Layer

The 1986 commitment was the **optimization-layer enforcement** of the 1985 arithmetic lottery. Euclidean gradient descent (O(N) storage/compute) won because it was hardware-correct; natural gradient descent using the Fisher information matrix as Riemannian metric was theoretically correct but computationally prohibitive.

**2023–2026 reversal** (Sophia: 50% step reduction via diagonal Hessian; Muon: spectral-norm steepest descent; SOAP; FAdam) is the systematic recovery of curvature awareness. Muon’s Newton-Schulz iteration is literally a CORDIC-like fixed-point procedure on the matrix manifold.

---

### 3. The Three Ceilings — Where the Stack Breaks

- **Iteration Ceiling (2026–2028)**: Reasoning models bill in tokens/iterations; IEEE 754 bills in FLOPS.
- **Curvature Ceiling (2025–2027)**: Optimizer blindness to Fisher geometry.
- **Biology Compute Ceiling (2028)**: $490B annual architectural waste.

All three are simultaneously addressable by geometry-native + CORDIC-native + curvature-aware infrastructure.

---

### 4. The Representational Bundle Hypothesis (RBH) — What the Stack Is Computing

The trained Transformer computes a **sloppy hyperribbon manifold** that is the total space of a principal SO⁺(1,𝑛)-bundle over a Lorentzian-stratified token base, with attention serving as the connection one-form (RBH, 2026 synthesis).

- Horizontal (stiff) directions = base-manifold Lorentzian geometry (transfers across tasks)
- Vertical (sloppy) directions = polytopal fiber geometry (task-specific)
- Chain-of-thought = path lifting
- Grokking = holonomy accumulation
- ICL = bundle holonomy scaling

---

### 5. CORDIC Revival — Closing the Arithmetic Loop

The 1959 CORDIC algorithm (Volder) that lost the 1985 lottery is now the native substrate for:
- Hyperbolic/Lorentzian operations
- Fixed-point iteration (reasoning, diffusion, Sinkhorn)
- Resource-efficient accelerators

Recent breakthroughs:  
**CARMEN** (arXiv:2605.06878, 2026) — CORDIC-accelerated Riemannian engine  
**“CORDIC Is All You Need”** (arXiv:2503.11685, 2025)  
TREA, CORVET, and multiple FPGA/edge designs (2025–2026).

This is the arithmetic reversal that simultaneously solves the iteration, curvature, and biology ceilings.

---

### 6. The Lorentzian Transition — Market Sizing & Action Agenda

**Conservative addressable market (20% SOM):**  
2027: ~$16B → 2028: ~$28B → 2030: ~$53B

**Immediate (Q1–Q2 2027):**  
- Geometric audit of stack  
- Instrument attention curvature telemetry  
- Fix grokking capital allocation errors

**Near-term (Q3 2027–2028):**  
- Launch Lorentzian prototype in one high-value hierarchical domain  
- Reassess procurement against geometry-native silicon (CORDIC + curvature primitives)

---

### 7. Ten Falsifiable Predictions

P1. Frontier silicon quotes iteration-rate (denoising-steps/s) alongside FLOPS by 2028.  
P2. Muon-class optimizer becomes default for hidden layers by 2027.  
P3. ≥3× step reduction via information-geometric preconditioning on 7B models by 2027.  
P4–P10 (full list in original reports) cover grokking holonomy, polytopal recovery, Lorentzian metrics in production, biology cost reduction ≥5×, and recognition of the Gradient Descent Lottery framing.

---

### Evidence Base & Sources

**Core references** (selected; full bibliographies in linked repositories):

- Hooker, S. *The Hardware Lottery* (2020) arXiv:2009.06489
- Rumelhart et al. *Nature* (1986)
- Vaswani et al. arXiv:1706.03762 (2017)
- Amari, S.-I. *Neural Computation* (1998)
- Liu et al. Sophia (ICML 2024, arXiv:2305.14342)
- He et al. HELM (NeurIPS 2025, arXiv:2505.24722)
- Kumar et al. CARMEN (arXiv:2605.06878, 2026)
- Robinson et al. (arXiv:2410.08993 & arXiv:2504.01002)
- Power et al. Grokking (arXiv:2201.02177)

**Full repositories:**  
[Geometry of Compounding Advantage](https://github.com/ericrenone/The-Geometry-of-Compounding-Advantage)  
[Gradient Descent Lottery](https://github.com/ericrenone/The-Gradient-Descent-Lottery)

---

**“The data was curved. The substrate was flat. The optimizer was charged with moving through the former on the geometry of the latter. The bill has been paid in steps. The reversal compounds in the opposite direction.”**

— Eric Ren, 2026–2027

*Last updated: May 2026*  
© 2026 Eric Ren (ericrenone) · CC-BY-SA 4.0 (non-commercial analysis; commercial implementations encouraged with attribution)

*Star this repo if you are building the next geometric infrastructure moat.*
