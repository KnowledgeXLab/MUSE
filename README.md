

<a name="readme-top"></a>

<div align="center">  
  <img src="misc/teaser.png" alt="MUSE Logo" width="420" style="background-color:white; display:inline-block; padding:8px;">  
</div>  

# 🧠 MUSE: A Memory-Utilizing and Self-Evolving Agent


> **Towards Self-Evolving Agents: Enabling Autonomy through Interactive Experience Refinement**  
> 📄 [ACL 2026 Findings](https://aclanthology.org/2026.findings-acl.1522.pdf)

---

## ✨ Abstract  

Large Language Models have demonstrated remarkable capabilities across diverse domains, yet significant challenges persist when deploying them as AI agents for real-world long-horizon tasks. Existing LLM agents suffer from a critical limitation: they are test-time static and cannot learn from experience, lacking the ability to accumulate knowledge and continuously improve on the job. To address this challenge, we propose MUSE, a novel agent framework that introduces an experience-driven, self-evolving system centered around a hierarchical Memory Module. MUSE organizes diverse levels of experience and leverages them to plan and execute long-horizon tasks across multiple applications. After each sub-task execution, the agent autonomously reflects on its trajectory, converting the raw trajectory into structured experience and integrating it back into the Memory Module. This mechanism enables the agent to evolve beyond its static pretrained parameters, fostering continuous learning and self-evolution. We evaluate MUSE on the long-horizon productivity benchmark TAC. It achieves new SOTA performance by a significant margin using only a lightweight Gemini-2.5 Flash model. Sufficient Experiments demonstrate that as the agent autonomously accumulates experience, it exhibits increasingly superior task completion capabilities, as well as robust continuous learning and self-evolution capabilities. Moreover, the accumulated experience from MUSE exhibits strong generalization properties, enabling zero-shot improvement on new tasks. MUSE establishes a new paradigm for AI agents capable of real-world productivity task automation.

---

## 🏆 Benchmark Performance

MUSE ranks **#1** on [The Agent Company Benchmark Leaderboard](https://the-agent-company.com/#/leaderboard).

<div align="center">  
  <img src="misc/TAC_rank1.png" alt="TAC Rank" width="500">  
</div>  

---

## 🚀 Quick Start

### Step 1: Environment Setup

```bash
conda create -n MUSE python=3.12
conda activate MUSE
pip install -r requirements.txt
playwright install chromium
playwright install-deps chromium
```

### Step 2: Run Local Demo

```bash
python demo.py
```

---

## 🧪 Run TAC Benchmark

To evaluate MUSE on **The Agent Company Benchmark**, please follow the detailed setup in:
👉 [TheAgentCompanyForMuse Repository](https://github.com/KnowledgeXLab/TheAgentCompanyForMuse)

---

## 🎥 Demo Showcase

**Task 1:** *HR - Internal Tooling Slides*

<p align="center">
  <a href="https://www.youtube.com/watch?v=8pK3SP0ZG4k&feature=youtu.be">
    <img src="misc/demo1.png" alt="Watch Demo 1" width="320" style="border-radius:12px;">
  </a>
</p>

**Task 2:** *PM - Updates Plane Issue from GitLab Status*

<p align="center">
  <a href="https://www.youtube.com/watch?v=hsM0FB9uVhs&feature=youtu.be">
    <img src="misc/demo2.png" alt="Watch Demo 2" width="320" style="border-radius:12px;">
  </a>
</p>

