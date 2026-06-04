<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=180&section=header&text=Naveen%20Kumar%20B%20A&fontSize=42&fontColor=fff&animation=twinkling&fontAlignY=32&desc=Senior%20Lead%20Engineer%20%7C%20Physical%20AI%20%7C%20Foundation%20Models%20%7C%20Autonomous%20Driving&descAlignY=62&descSize=16" width="100%"/>

<p align="center">
  <a href="mailto:basaanithanaveenkumar1998@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white"/></a>
  <a href="https://linkedin.com/in/basaanithanaveenkumar" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
  <a href="https://github.com/basaanithanaveenkumar" target="_blank"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"/></a>
  <img src="https://komarev.com/ghpvc/?username=basaanithanaveenkumar&style=for-the-badge&color=blueviolet" alt="Profile Views"/>
</p>

<br/>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=6AD3F7&center=true&vCenter=true&width=700&lines=Building+Foundation+Models+for+Physical+AI;VLA+%7C+World+Action+Models+%7C+E2E+Driving;Autonomous+Driving+%7C+3D+Perception+%7C+BEV;From+First+Principles+to+Production" alt="Typing SVG" />
</p>

---

## About Me

I architect and build **multi-modality foundation models for Physical AI** — spanning the full stack from raw sensor data to deployed policies running on vehicle SoCs. My work sits at the intersection of **2D/3D Perception**, **End-to-End driving stacks**, and **Vision-Language-Action (VLA)** systems that reason about the world before they act.

I design from first principles. When I build a model, I understand every layer — from tokenization strategies and attention variants to training dynamics and inference optimization for real-time hardware. I have applied this depth at **BMW Techworks** and **Mercedes-Benz R&D**, where I led teams building production autonomous driving systems, and shipped work that runs inside real vehicles.

Beyond perception and planning, I am actively developing **HALO** — a personal series of foundation models built entirely from scratch: a World Action Reasoning Model, a VLA, and a VLM — each designed to push the frontier of embodied intelligence.

Multi-awarded inventor with patents filed across the US, EP, and AU, and a published trajectory prediction paper.

---

## Where I Have Worked

<table>
<tr>
<td width="60px" align="center"><b>🚗</b></td>
<td>
<b>BMW Techworks India</b> — Senior Lead Engineer & Assistant Manager, Automated Driving<br/>
<sub>Oct 2025 – Present · Bangalore, India</sub><br/><br/>
Leading architecture and implementation of a Sparse BEV-based End-to-End autonomous driving stack — owning the complete loop from data curation through policy training. Pioneered an embodied VLM-powered Scene Mining agent that intelligently indexes safety-critical scenarios directly feeding the continuous retraining pipeline. Enabling natural language command-based contextual responses from historical observations through VLM-powered autonomous capabilities.
</td>
</tr>
<tr><td colspan="2"><br/></td></tr>
<tr>
<td width="60px" align="center"><b>⭐</b></td>
<td>
<b>Mercedes-Benz Research & Development India</b> — Perception Engineer, L3 Automated Driving<br/>
<sub>Jun 2023 – Sep 2025 · Bangalore, India</sub><br/><br/>
Contributed to the self-driving stack powering next-generation Mercedes-Benz vehicles (CLA and new releases). Designed and trained multi-modality foundation models fusing Camera, LiDAR, RADAR, and language for autonomous driving agents that reason before acting. Architected an E2E AD foundation model fusing self-supervised learning, imitation policy, and 4D semantic occupancy. Closed the data-to-deployment loop by integrating unified models onto Nvidia Orin for cross-platform vehicle SoC deployment.<br/><br/>
<sub>🏆 Bronze Star Award — Revolutionized cross-functional collaboration and reengineered workflows to slash operational costs.</sub><br/>
<sub>🏆 PAC Award — Recognized as lead inventor on multiple patents driving breakthrough intellectual property.</sub>
</td>
</tr>
<tr><td colspan="2"><br/></td></tr>
<tr>
<td width="60px" align="center"><b>🔬</b></td>
<td>
<b>TCS Research & Innovation Labs</b> — Research ML Developer, Sensorium.ai<br/>
<sub>Feb 2021 – Jun 2023 · Bangalore, India</sub><br/><br/>
Built and shipped a wide range of production-grade computer vision models across environmental AI — detection of bleeds, canopy changes, vegetation encroachment, flood events, snow, and more. Pioneered an uncertainty-aware Active Learning auto-annotation framework. Developed the SenSat and SenCV libraries to accelerate satellite and CV pipelines. Mentored engineers building ecological intelligence solutions fusing SAR, Hyperspectral, and DEM sensors.<br/><br/>
<sub>🏆 IP Creation Award — Spearheaded high-impact patent filings in autonomous vision systems.</sub>
</td>
</tr>
</table>

---

## Personal Projects — Foundation Models Built from Scratch

> These are not fine-tuned wrappers. Every architecture decision, every training objective, every component — engineered from first principles.

<table>
<tr>
<td valign="top" width="50%">

### 🌐 HALO-WARM
**World Action Reasoning Model**

Custom Transformer Decoder with three-stream tokenization across vision, language, robot state, and world query tokens. Mixture-of-Experts architecture with shared and routed experts per layer. Multi-output heads spanning language reasoning, action decoding, future depth prediction, future frame prediction, and future flow prediction. Currently adding model-based RL fine-tuning using imagined futures as a training environment for policy optimisation via PPO.

</td>
<td valign="top" width="50%">

### 🤖 HALO VLA
**Vision-Language-Action Model**

Built from scratch with a **Flow Matching Action chunking Decoder** — replacing standard action heads to model continuous robot action sequences with smooth, natural trajectories. Designed for real robot deployment where trajectory quality directly determines task success.

</td>
</tr>
<tr>
<td valign="top" width="50%">

### 👁️ HALO VLM
**Vision-Language Model**

Custom ViT and Transformer Decoder from scratch with causal masking and autoregressive generation. Sparse Mixture-of-Experts layer (DeepSeek-inspired) with custom routing and load balancing. Multi-Token Prediction for simultaneous n-future token generation, enabling dramatically faster inference. Gradient checkpointing to cut VRAM footprint significantly.

</td>
<td valign="top" width="50%">

### 🧩 VL-JEPA
**Joint Embedding Predictive Architecture**

World model that learns abstract representations by predicting masked patches of visual and linguistic inputs entirely in latent space — no pixel-level or token-level reconstruction. Pure latent-space learning of the structure of the visual-linguistic world.

</td>
</tr>
<tr>
<td valign="top" width="50%">

### 🌿 DINO from Scratch
**Self-Supervised Visual Representation**

Full teacher-student self-distillation framework (Self-Distillation with No Labels) that learns high-quality visual features without any annotations. Pure self-supervised learning from raw visual signal.

</td>
<td valign="top" width="50%">

### 🍎 Agri-Sort Grading System
**360° Real-Time Vision Pipeline**

State-memory vision algorithm with full 360° real-time perception for sorting and grading produce by size, shape, colour, weight, and surface quality. Transformed throughput from a small-scale manual operation to a high-volume automated pipeline.

</td>
</tr>
</table>

---

## Patents & Publications

| Type | Title |
|------|-------|
| 📄 **Paper** | *Map-Less Yet Accurate: Trajectory Prediction for Traffic Agents Using Online HD Map Reconstruction* |
| 🔒 **Patent** (US, EP, AU) | Autonomous task composition of vision pipelines using an algorithm selection framework |
| 🔒 **Patent** | Robust Vehicle Radar System — Automatic Clutter Removal |
| 🔒 **Patent** | Robust Lidar PCD for Moderate Weather |
| 🔒 **Patent** | Tunnel Map Generation with Adaptive Neural Compression |
| 🔒 **Patent** | Context-Aware ADAS Adaptation through VLM — Multimodal Behavioural Analytics |

---

## Technical Expertise

### Foundation Models & AI Architectures
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![CUDA](https://img.shields.io/badge/CUDA-76B900?style=flat-square&logo=nvidia&logoColor=white)
![ONNX](https://img.shields.io/badge/ONNX-005CED?style=flat-square&logo=onnx&logoColor=white)
![TensorRT](https://img.shields.io/badge/TensorRT-76B900?style=flat-square&logo=nvidia&logoColor=white)

**VLA · VLM · World Action Models · Diffusion Models · Flow Matching · DiT · MoE · ViT · BEVFormer · BEV-Det**

### Autonomous Driving & Perception
**End-to-End Driving Stacks · BEV Perception · 3D Object Detection · Trajectory Prediction · 4D Semantic Occupancy · Multi-Camera Fusion · LiDAR · RADAR · HD Maps · SLAM · Multi-View Geometry**

### Training & Optimization
**LoRA / QLoRA · QAT · Latency-Aware In-Training Pruning · Neural Architecture Search · Mixed Precision · Knowledge Distillation · Weight Sharing · Sensor Dropout · Large-Scale Distributed Training (HPC · A100 clusters)**

### Agentic & Generative AI
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI_SDK-412991?style=flat-square&logo=openai&logoColor=white)

**RAG · LangGraph · CrewAI · Embodied Agents · Scene Mining Pipelines**

### Languages & Tools
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=c%2B%2B&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![ROS](https://img.shields.io/badge/ROS-22314E?style=flat-square&logo=ros&logoColor=white)

---

## GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=basaanithanaveenkumar&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0D1117&title_color=6AD3F7&icon_color=6AD3F7&text_color=c9d1d9" height="165"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs?username=basaanithanaveenkumar&layout=compact&theme=tokyonight&hide_border=true&bg_color=0D1117&title_color=6AD3F7&text_color=c9d1d9" height="165"/>
</p>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com?user=basaanithanaveenkumar&theme=tokyonight&hide_border=true&background=0D1117&ring=6AD3F7&fire=FF6B6B&currStreakLabel=6AD3F7" width="60%"/>
</p>

---

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=100&section=footer" width="100%"/>
