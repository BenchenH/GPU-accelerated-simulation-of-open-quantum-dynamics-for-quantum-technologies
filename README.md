# TUT::QSIMU::QTEM::123 — GPU-accelerated simulation of open quantum dynamics for quantum technologies

**IEEE Quantum Week 2026 (QCE26) — Tutorial**

Real-world quantum systems are subject to external interactions, whether intentional or unintentional. These interactions underpin the fundamental processes that drive experimental observations. Accurate simulations of **open quantum systems (OQS)** provide crucial insight into these processes and serve as a design tool for building high-quality quantum processors — letting researchers navigate the complex parameter space of hardware and develop more precise control and readout techniques.

In this hands-on tutorial we perform OQS simulations on **AWS**, using **CUDA-Q Dynamics** and **QuTiP** (with the **qutip-cuquantum** plugin), and validate our simulation results against a real superconducting quantum processing unit on **Amazon Braket**. Participants leave with practical code examples they can build on for their own research and projects.

---

## Presenters

- **Benchen Huang** — Amazon Web Services
- **Sebastian Stern** — Amazon Web Services
- **Tyler Takeshita** — Amazon Web Services
- **Jin-Sung Kim** — NVIDIA
- **Boris Varbanov** — University of Sherbrooke

---

## Target audience

Students, researchers, and engineers in computer science, quantum computing, quantum information science, and HPC. Academic and industry researchers gain a practical understanding of OQS simulation toolkits and how to architect HPC resources on the cloud. Students and the broader audience learn best practices for using cloud-based quantum computing services on AWS.

---

## What you'll leave with

- Working code that runs single-qubit gate simulations in **CUDA-Q Dynamics** and **QuTiP**.
- A reproducible **CPU vs GPU** benchmark for open-system dynamics on cloud infrastructure.
- A pulse-level experiment on a real superconducting QPU accessed through **Amazon Braket**.
- A complete set of Jupyter notebooks you can adapt to your own hardware-design workflows.

Complimentary access to temporary AWS accounts is provided during the tutorial.

---

## Agenda

The tutorial runs in **two 90-minute sessions with a lunch break in between**.

### Session 1 — foundations and simulation

| Slot | Content |
|---|---|
| **20 min** | **Presentation:** Tutorial overview<br>• Overview of AWS services and tools<br>• Access Workshop Studio accounts |
| **30 min** | **Presentation:** Open quantum systems basics<br>• Brief review of open quantum dynamics<br>• Introduction to the superconducting qubit |
| **30 min** | **Hands-on lab:** Modeling superconducting qubits using CUDA-Q Dynamics<br>• Introduction to CUDA-Q Dynamics |

---

### Session 2 — applications on AWS and validation on hardware

| Slot | Content |
|---|---|
| **20 min** | **Presentation:** Introduction to Amazon Braket |
| **40 min** | **Hands-on lab:** Optimizing single-qubit rotation pulse sequences<br>• Introduction to QuTiP<br>• Comparing Gaussian vs DRAG pulse schemes in single-qubit rotation<br>• Validation on a real superconducting QPU on Amazon Braket |
| **20 min** | **Hands-on lab:** Optimizing drive strength in dispersive readout<br>• CPU vs GPU runtime benchmarks |

---

## Prerequisites

- **Familiarity with Python and Jupyter notebooks.** All hands-on labs are provided as notebooks.
- **Basic quantum-mechanics background.** Density matrices, Hamiltonians, Lindblad master equations. A brief refresher is provided in the OQS-basics presentation.
- **No prior experience** with CUDA-Q, QuTiP, or Amazon Braket is required.

Bring a laptop with a modern web browser. All hands-on execution happens in the cloud through AWS Workshop Studio — no local installation required.

---

## What you'll build

Over the course of the tutorial, you will:

1. **Simulate a driven transmon** in CUDA-Q Dynamics — the standard superconducting qubit model.
2. **Design single-qubit gates in QuTiP.** Compare Gaussian and DRAG pulse shapes, understand the leakage-vs-decoherence tradeoff, and identify the pulse-design regime hardware manufacturers use in production.
3. **Verify your design on real hardware.** Submit an Amazon Braket hybrid job to a Rigetti Cepheus superconducting QPU, comparing custom pulse sequences at the pulse level.
4. **Optimize dispersive readout** by exploring the weak-vs-strong-drive tradeoff. Benchmark the same simulation on CPU vs GPU.

The tutorial's physics is honest to modern superconducting quantum hardware — parameter choices match those used at IBM, Google, Rigetti, and Amazon Braket-accessible devices.

---

## Contact

For questions about the tutorial, contact the organizers through the [IEEE Quantum Week 2026 program page](https://qce.quantum.ieee.org/2026/qce26-schedule/qsimu-schedule/).

For issues with the tutorial materials, please open an issue on this repository.
