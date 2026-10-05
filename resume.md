# NAVEENKUMAR B A

basaanithanaveenkumar@gmail.com | +91-9704041804 | [GitHub](https://github.com/basaanithanaveenkumar) | [LinkedIn](https://linkedin.com/in/basaanithanaveenkumar) | Bangalore, India (Open to relocate)

## Professional Summary

- Senior Lead Engineer with 6+ years of experience architecting and shipping Perception and multi-modal foundation models for Physical AI.
- Proven expertise across 3D/2D Perception, pre-training, and fine-tuning Vision Language Action (VLA) & World Action Models (WAM).
- Multi-awarded innovator with patents and publications, recognised for consistent delivery of Pareto frontier of accuracy vs latency.

## Experience

### BMW Techworks - Bangalore, India | Oct 2025 - Present
**Senior Lead ML Engineer & Assistant Manager - Automated Driving & Embodied AI**

**Leadership**
- Led a cross-functional team of 5 (Perception & Planning) to evaluate emerging VLA and world-model technologies for AD/robotics; delivered CXO-level strategic briefings that shaped the corporate roadmap.

**World Model & Planning**
- **Sparse BEV World Model:** Owned the full data-to-policy pipeline for a Sparse BEV world model across 4.8M multi-camera scenes, leading a team of 4 across perception and planning; implemented BEV latent world-model training as auxiliary representation learning aligned to future frames — 56% improved open-loop metrics (ADE, missrate, FDE) and ~34% fewer closed-loop collisions.
- **World Model-Guided RL Planning:** Used a Sparse BEV world model to score candidate trajectories, producing reward signals for closed-loop RL fine-tuning of the planning policy — 63% reduction in closed-loop collision rate - directly improving safety margins, +7.1 PDMS over the imitation baseline.
- **BEV Spatial Importance:** Built an adaptive BEV spatial selector, replacing computationally heavy dense BEV feature maps with navigation-conditioned query tokens, it uses high-level navigation intent to dynamically direct model attention strictly to relevant scene elements. 2.5x inference speedup.
- **Multi-Frame Temporal Fusion:** Fused BEV features across multiple frames to strengthen scene-level context for both detection and segmentation heads — 27% mAP gain on multi-task 3D detection, 25% mIoU gain on BEV segmentation.

**3D Perception & Auto-Labeling**
- **3D Obstacle Perception:** Refined architecture, augmentation and training recipe for multi-modal 3D obstacle detection — 24% mAP improvement.
- **Auto-Labeling Pipeline:** Engineered an ensembled-supervision labelling pipeline for 3D obstacle detection achieving 72% mAP parity with human annotators; cut annotation cost by €1.2M (97%), feeding a data flywheel after verification.
- **3D-GS View Synthesis:** Built a synthetic data generation pipeline using 3D Gaussian Splatting to reconstruct driving scenes and render photorealistic novel views across target vehicle variants — 45% mAP gain on new hardware without a single real-world collection run.
- **Intelligent Model Selector:** Engineered an inference routing to dynamically select the optimal model variant per scenario, cutting €280K in compute costs.

**Vision-Language Scene Understanding**
- **VLAM Contextual Reasoning:** Built VLAM-powered capabilities enabling natural-language command-based contextual responses grounded in historical observations, delivered through cross-functional collaboration with platform and planning teams.
- **BEV-CLIP:** Extended contrastive vision-language pretraining from image space to BEV latent space to address standard CLIP's failure on spatial reasoning — enables ego-centric object-relation queries and occlusion-aware scene retrieval for safety-critical mining.
- **VLM Data Curation Agent:** Auto-surfaces failure cases and safety-critical edge cases into retraining pipelines — 95% reduction in manual curation; fused behavioral cues into the retrieval signal (+37% tagging accuracy), with a caching layer that lifted throughput by 70%.
- **Model Ingestion Framework:** Engineered a plug-and-play Factory Method framework for model variant onboarding, cutting integration turnaround by 60%.

### Mercedes-Benz Research & Development India - Bangalore, India | Jun 2023 - Sep 2025
**Machine Learning Engineer - L3 Automated Driving**

**Foundation Models & End to End Planning**
- **VLAM:** VLA pre-training from scratch on a multi-modal, multi-embodiment corpus (Camera, LiDAR, RADAR, language trajectories) for long-horizon embodied action reasoning; trained the base policy via behavior cloning, then ran systematic scaling experiments (depth × width, MoE) to locate the capacity–latency Pareto point — custom loss function and instruct-tuning drove 57% improvement in VLA planning metrics.
- **End to End Driving Model (AV2.5):** Architected an end-to-end driving policy fusing self-supervised learning with an imitation policy over a 4D semantic occupancy network — 48% relative improvement in vehicle-in-the-loop planning metrics; applied NAS for 50% model compression at <4% accuracy loss, and a custom loss on the prior AV2.0 model delivered a 67% relative planning-metric boost.
- **Trajectory Prediction:** Built a VRU trajectory predictor fusing perceptual features with HD map via attention — 18% improvement in Prediction metrics.
- **Proximity-Based Safety Prediction Metric:** Co-developed a safety-aware trajectory evaluation metric — extending Brier-minFDE with distance- and relevance-weighted heuristics — to better capture near-field, safety-critical planning risk that standard metrics understate; published at SAE 2026.
- **HD Map Generation (Vectorized):** Engineered architectural refinements to a transformer-based online HD map reconstruction model, delivering a 17% boost in mAP over the baseline through targeted enhancements to the decoder's cross-attention and query design.

**Recognition & Cross-Functional Impact**
- Drove cross-functional process innovation that reduced $240K in compute cost. Collaborated across teams to deploy generative models (transformers, flow-matching) for CV and NLP applications; delivered executive tech-trend briefings that informed proactive technology adoption.

**3D Perception & Deployment - models running in production on CLA**
- **Multi-Camera 3D Detection:** Improved mAP by 57% with long-range gains (120–200m+), extending operating envelope at highway speeds (>100 km/h).
- **BEV Free-Space Detection:** Improved free-space detection by 19% at 120-200m range, giving the planner a more reliable drivable-area boundary at distances where early lane-change and merge decisions are made — directly reducing downstream planning uncertainty at highway speeds.
- **Inference Optimization:** Optimized models for real-time edge inference on Nvidia Drive Orin using latency-aware in-training pruning, QAT, and TensorRT compilation — 2.78x speedup meeting hard on-vehicle latency constraints; deployed to production on the Mercedes-Benz CLA platform.
- **Cross-Vehicle Unification:** Trained a single unified model generalizing across multiple vehicle variants rather than per-variant models.
- **Sensor-Dropout Robustness:** Trained with randomized sensor dropout to harden perception against single-point failures, improving mAP by 17%.
- **Large-Scale Training:** Trained and optimized DNNs on a petabyte-scale, 15M multi-camera scene dataset across 512+ A100 GPUs using data parallelism with gradient sharding, mixed precision (FP16), Quantization-aware training (QAT), latency-aware pruning, weight-sharing to maximize hardware efficiency.

### TCS - Research & Innovation Labs - Bangalore, India | Feb 2021 - Jun 2023
**Research ML Developer - Sensorium.ai**

**Multimodal Model Development**
- **Reusable Models:** Shipped 12+ production-grade cross-modal CV models as a shared library — 40% faster dev cycles at >92% accuracy; built an uncertainty-aware active-learning auto-annotation framework achieving 90% reduction in manual labeling.

**Platform & Infrastructure**
- **SenSat & SenCV Libraries:** Built internal satellite/CV libraries - self-supervised pretraining, standardizing model development.
- **Geo-Spatial AI:** Scaled inference infrastructure via tiling (7× faster processing, 2.7× faster data-fetch) across NASA/ESA/Maxar; Model Engine with data caching drove 4× throughput gain.

**Mentorship & Applied Research**
- Mentored 8 engineers on multi-sensor fusion (SAR / hyper-spectral / DEM) and domain adaptation across tree health, carbon sequestration, and P&C analytics — building bench depth beyond immediate project scope.

### Quantrium Tech | Nov 2020 - Feb 2021
**Machine Vision Intern**
- Developed Auto Image Skew & Orientation Correction, print enhancer for bank passbook with 97.7% accuracy.

## Publications & Patents

- **Paper:** Map-Less Yet Accurate: Trajectory Prediction for Traffic Agents Using Online HD Map Reconstruction — SAE Technical Paper 2026-26-0039, SAE International (2026). saemobilus.sae.org/content/2026-26-0039
- **Patent:** Autonomous task composition of vision pipelines using an algorithm selection framework (US, EP, AU) — Co-invented a symbolic planner that maps a task into subtasks, then a transformer with Proximal policy (PPO) scores and picks the best algorithm.
- **Patent:** Robust Vehicle Radar System - Automated Clutter Removal — Developed automatic clutter-removal system using sensor supervision, reducing manual fine-tuning effort by 80%.
- **Patent:** Robust Lidar PCD for Moderate weather — Enhanced LiDAR point-cloud quality by filtering 96% of environmental clutter under moderate weather conditions.
- **Patent:** Systems and Methods for generating Map data for vehicle in Network outage regions — Pioneered generation of HD Maps in Network outage regions like Tunnels with neural data compression, achieving 10x map storage reduction.
- **Patent:** Context aware ADAS adaptation through VLM - Multimodal Behavioural Analytics — Modeled occupant behavior and driver intent to enable personalized, comfort-aware ADAS responses conditioned on individual user context.

## Skills

- **Languages:** Python, C/C++, Java, Rust
- **Foundation Models:** Vision-Language-Action (VLA) models, VLM, World Action Models (WAM), OpenVLA, Groot, π0, π0.5, CLIP
- **AI/ML Frameworks & Libraries:** PyTorch, Tensorflow, OpenCV, TensorRT, ONNX, HuggingFace, Transformers, Numpy, CUDA, Open3D, DeepSpeed, Ray
- **AI Concepts & Architectures:** Deep Learning, Computer Vision, Reinforcement Learning (DPO, PPO, GRPO, RLHF), NLP, Transformers, Vision Language Models (VLM), Mixture of Experts (MoE), Multi-modal fusion, Cross-Modal attention, Multi Query Attention, Grouped Query Attention, Gated attention, Vision Transformers (ViT), 2D to BEV (BEVformer, BEV-DET), Multi-View Geometry, SLAM, Knowledge Distillation, SfM, Diffusion Transformer (DiT), Diffusion, Flow Matching
- **AI Training & Optimization:** Parameter-Efficient Fine-Tuning (PEFT) - (LoRA, QLoRA), Neural Architecture Search (NAS), KV caching, Post training Quantization (INT8), Pruning - Latency aware In-Training pruning, FSDP, ZeRO 1/2/3, Large-Scale Data Pipelines, ML-Ops, torchtitan, 4D parallelism
- **Leadership & Domain:** Stakeholder Briefings, Cross-functional Team Leadership, ADAS, Robotics, LiDAR, 4D-Radar, Multi/Hyper-Spectral Imaging
- **AI & Engineering:** LangChain, LangGraph, CrewAI, RAG, Git, Linux, Docker, ROS 2, Cloud, HPC

## Projects

### Personal Projects | Foundation Models: Built from Scratch

**HALO-WARM — World Action Reasoning Model, built from scratch**
Designed and training a unified world+action model.
- **Three-Stream MoE Transformer Decoder:** Engineered a 12-layer decoder with separate vision, language, robot-state, and world-query token streams feeding a Mixture-of-Experts backbone (2 shared + 12 routed experts/layer) with four output heads (language reasoning, action decoding, DiT future-frame prediction, future flow) — routing keeps only ~106M of 393M total parameters active per forward pass.
- **World Model for Post Training:** Trained the world model as pre-training objective — predicting future frames and future depth via the DiT decoder. Froze the trained world model and repurposed it as a learned simulator — rolling out imagined trajectories through the DiT decoder, scoring them with latent-space rewards, and updating the action head via PPO — avoiding the cost and risk of real-environment rollouts entirely.
- **Delta-Token World Compression:** Compressed world representations into delta tokens rather than full dense states, reducing redundant world-state encoding across time steps.

**HALO VLA — Vision-Language-Action Model for Humanoid, built from scratch**
Rethinking the action head to fix jerky, discontinuous robot trajectories.
- **Flow matching Action chunking Decoder:** Replaced the standard MLP action head with a conditional flow matching decoder that predicts action chunks as continuous trajectories, improving multimodal trajectory smoothness (inspired from π0).

**HALO VLM — Vision-Language Model, built from first principles**
Custom ViT + decoder stack optimized for both capacity and inference speed.
- **Custom ViT + Causal Decoder from Scratch:** Engineered a from-scratch Vision Transformer paired with a 16-layer causal transformer decoder, implementing masked autoregressive text generation without relying on pretrained backbones.
- **Sparse MoE Routing (DeepSeek-inspired):** Integrated a sparse Mixture-of-Experts layer with custom routing and load-balancing losses — expanding model capacity without the proportional compute cost of a dense model of equivalent size.
- **Multi-Token Prediction for Inference Speed:** Shifted decoding from sequential next-token prediction to simultaneous n-future-token prediction, cutting the number of forward passes needed per output sequence — 3x faster inference.
- **Activation Checkpointing for Memory:** Swapped storing all intermediate activations for on-demand recomputation during backprop — trading extra compute for memory — 66% VRAM reduction.

**Self-Supervised DINO - PreTraining from Scratch**
Learning visual features without any labels.
- **Teacher-Student Self-Distillation:** Implemented DINO's EMA-updated teacher-student annotation-free visual representation learning via self-distillation.

**HALE-LLM — Unified Multi-Paradigm Language Model, built from scratch**
An incremental journey from a plain autoregressive transformer to a registry of five interchangeable generation paradigms.
- **Autoregressive Foundation from Scratch:** Started with a from-scratch decoder-only transformer trained with standard next-token prediction — no pretrained weights, no borrowed reference implementation — establishing the shared trunk that every later paradigm would plug into.
- **Activation Checkpointing for Memory Headroom:** Hit VRAM limits scaling depth on a single machine, so swapped full activation storage for on-demand recomputation during backprop — trading extra compute for the memory headroom needed to keep scaling the trunk.
- **DeepSeek-Style Mixture-of-Experts:** Replaced the dense FFN with a sparse MoE layer (shared + routed experts, custom load-balancing loss) — expanding model capacity without paying the proportional compute cost of a same-size dense model.
- **MQA → GQA Attention Redesign:** Reworked attention from standard multi-head to multi-query, then settled on grouped-query attention — sharing key/value projections across head groups to shrink the KV-cache footprint without collapsing attention expressivity the way full MQA does.
- **Multi-Token Prediction Head:** Added parallel prediction heads to forecast several future tokens per forward pass instead of one, cutting the number of sequential decoding steps needed at inference.
- **Masked Diffusion LM Variant:** Stepped outside autoregression entirely — implemented a masked diffusion head that corrupts and iteratively denoises the full sequence, trading strict left-to-right generation for parallel refinement.
- **Block Diffusion (BD3-LM style):** Bridged the two paradigms — generates fixed-size blocks autoregressively across blocks while denoising tokens within each block via diffusion, preserving KV-cache reuse while still getting intra-block parallelism.
- **Unified Registry Architecture:** Rather than maintaining these as separate one-off models, refactored all variants — AR, MoE, MTP, masked diffusion, block diffusion, plus flow matching and block flow matching — into pluggable heads registered against one shared backbone, packaged as a uv-managed Python framework for apples-to-apples comparison.

**Agri-Sort Grading System**
Real-time multi-attribute sorting at production line speed.
- **360° Vision with State Memory:** Built a vision pipeline with persistent state memory and full 360° real-time perception to grade produce by size, shape, color, weight, and surface quality simultaneously — 400% throughput boost (700 → 2,800 units/hour).

## Awards

- Bronze Star Award (MBRDI) – Reengineered workflows to slash operational costs by an unprecedented 70%.
- PAC Award (MBRDI) – Recognized as lead inventor on multiple patents, driving breakthrough intellectual property.
- IP Creation Award (TCS) – Spearheaded high-impact patent filings in autonomous vision systems, cementing AI-driven perception.
- Team Excellence Award - BMW Techworks

## Education

**Madanapalle Institute of Technology and Science** - Madanapalle, India | 2017 - 2020
- B.Tech - Electronics and Communication | CGPA: 8.96

## Certifications

84+ Certifications from DeepLearning.ai, Coursera and Udemy including:
- Deep Learning Specialization (DeepLearning.AI) | Neural Nets & CNN
- ROS2 for Beginners (Udemy)
- LLMs Mastery (Udemy) | Transformers & GenAI
- Cutting-Edge AI: Deep Reinforcement Learning in Python (Udemy)
