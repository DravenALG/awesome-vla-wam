<div align="center">

# 🤖 Awesome VLA

**📜 A Curated List of Vision-Language-Action (VLA) Research** </br>

**🚀 Welcome to follow our exploratory work on VLA, [VLANeXt](https://github.com/DravenALG/VLANeXt).**

<p align="center">
  <img src="awesome-vla.jpg" alt="Awesome VLA" width="100%" style="border-radius: 15px; box-shadow: 0 4px 24px rgba(0,0,0,.1); margin: 5px 0;">
</p>

*Photo Credit: [Gemini-Nano-Banana🍌](https://aistudio.google.com/models/gemini-3-pro-image)*.

</div>

## Overview
- 🎯 [Aim](#aim)
- 📚 [Definition](#definition)
- 📖 [Survey](#survey)
- 🧠 [General VLA](#general-vla)
-  � [World Action Models in VLA](#world-action-models-in-vla)
- 💡 [VLA with Understanding and Reasoning](#vla-with-understanding-and-reasoning)
- 🌐 [VLA with 3D/4D Modelling](#vla-with-3d4d-modelling)
- 🔥 [VLA with Reinforcement Learning](#vla-with-reinforcement-learning)
- 🧪 [VLA with Latent Actions](#vla-with-latent-actions)
- 🪶 [Efficient VLA](#efficient-vla)
- 🧭 [Domain-Specific VLA (e.g., Humanoid, Tactile)](#domain-specific-vla-eg-humanoid-tactile)
- 🧷 [Other Topics in VLA](#other-topics-in-vla)
- 🦾 [Traditional Policies](#traditional-policies)
- 💾 [Datasets](#datasets)
- 📊 [Benchmark / Environment](#benchmark--environment)
- 🏞️ [Physics Engine](#physics-engine)
- 🖥️ [Hardware](#hardware)

## Aim
This is a curated list of VLA research that systematically organizes various topics within the field. It will be continuously updated and refined, with the goal of clarifying the research context for scholars in the VLA domain. If you have any new papers worth adding, please feel free to push and join us in maintaining a high-quality VLA list.

## Definition
In short, VLA models are a type of robotics policy that inherts the pretrained VLMs’ rich language grounding and visual understanding abilities to offter a scalable route toward general-purpose, language-conditioned robot policies. We can trace the origin and formal definition of the VLA to the work TR-2.

- [⭐️] **RT-2**, RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control. [![arXiv](https://img.shields.io/badge/arXiv-2307.15818-b31b1b.svg)](https://arxiv.org/abs/2307.15818) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://robotics-transformer2.github.io)

## Survey
- Vision-Language-Action (VLA) Models: Concepts, Progress, Applications and Challenges. [![arXiv](https://img.shields.io/badge/arXiv-2505.04769-b31b1b.svg)](https://arxiv.org/abs/2505.04769) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/Applied-AI-Research-Lab/Vision-Language-Action-Models-Concepts-Progress-Applications-and-Challenges)

- A Survey on Vision-Language-Action Models for Embodied AI. [![arXiv](https://img.shields.io/badge/arXiv-2405.14093-b31b1b.svg)](https://arxiv.org/abs/2405.14093) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/yueen-ma/Awesome-VLA)

## General VLA

- **SimVLA** SimVLA: A Simple VLA Baseline for Robotic Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2602.18224-b31b1b.svg)](https://arxiv.org/abs/2602.18224) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://frontierrobo.github.io/SimVLA/)

- **ABot-M0** ABot-M0: VLA Foundation Model for Robotic Manipulation with Action Manifold Learning. [![arXiv](https://img.shields.io/badge/arXiv-2602.11236-b31b1b.svg)](https://arxiv.org/abs/2602.11236) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://amap-cvlab.github.io/ABot-Manipulation/)

- [⭐️] **Lingbot-VLA** A Pragmatic VLA Foundation Model. [![arXiv](https://img.shields.io/badge/arXiv-2601.18692-b31b1b.svg)](https://arxiv.org/abs/2601.18692) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://technology.robbyant.com/lingbot-vla/)

- **VLM4VLA** VLM4VLA: Revisiting Vision-Language-Models in Vision-Language-Action Models. [![arXiv](https://img.shields.io/badge/arXiv-2601.03309-b31b1b.svg)](https://arxiv.org/abs/2601.03309) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://cladernyjorn.github.io/VLM4VLA.github.io/)

- Emergence of Human to Robot Transfer in Vision-Language-Action Models. [![arXiv](https://img.shields.io/badge/arXiv-2512.22414-b31b1b.svg)](https://arxiv.org/abs/2512.22414) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://www.pi.website/research/human_to_robot)

- [⭐️] **π∗0.6:**, π∗0.6: a VLA That Learns From Experience. [![arXiv](https://img.shields.io/badge/arXiv-2511.14759-b31b1b.svg)](https://arxiv.org/abs/2511.14759) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://www.pi.website/blog/pistar06)

- **VLA-0**, VLA-0: Building State-of-the-Art VLAs with Zero Modification. [![arXiv](https://img.shields.io/badge/arXiv-2510.13054-b31b1b.svg)](https://arxiv.org/abs/2510.13054) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://vla0.github.io)

- **UniVLA**, Unified Vision-Language-Action Model. [![arXiv](https://img.shields.io/badge/arXiv-2506.19850-b31b1b.svg)](https://arxiv.org/abs/2506.19850) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://robertwyq.github.io/univla.github.io/)

- **SmolVLA**, SmolVLA: A Vision-Language-Action Model for Affordable and Efficient Robotics. [![arXiv](https://img.shields.io/badge/arXiv-2506.01844-b31b1b.svg)](https://arxiv.org/abs/2506.01844) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/huggingface/lerobot)

- **NORA**, NORA: A Small Open-Sourced Generalist Vision Language Action Model for Embodied Tasks. [![arXiv](https://img.shields.io/badge/arXiv-2504.19854-b31b1b.svg)](https://arxiv.org/abs/2504.19854) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://declare-lab.github.io/nora)

- **CronusVLA**, CronusVLA: Towards Efficient and Robust Manipulation via Multi-Frame Vision-Language-Action Modeling. [![arXiv](https://img.shields.io/badge/arXiv-2506.19816-b31b1b.svg)](https://arxiv.org/abs/2506.19816) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://lihaohn.github.io/CronusVLA.github.io/)

- [⭐️] **Gemini Robotics**, Gemini Robotics: Bringing AI into the Physical World. [![arXiv](https://img.shields.io/badge/arXiv-2503.20020-b31b1b.svg)](https://arxiv.org/abs/2503.20020) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://deepmind.google/models/gemini-robotics/)

- [⭐️] **OpenVLA-OFT**, Fine-Tuning Vision-Language-Action Models: Optimizing Speed and Success. [![arXiv](https://img.shields.io/badge/arXiv-2502.19645-b31b1b.svg)](https://arxiv.org/abs/2502.19645) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://openvla-oft.github.io)

- [⭐️] **FAST**, FAST: Efficient Action Tokenization for Vision-Language-Action Models. [![arXiv](https://img.shields.io/badge/arXiv-2501.09747-b31b1b.svg)](https://arxiv.org/abs/2501.09747) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://www.pi.website/research/fast)

- **CogACT**, CogACT: A Foundational Vision-Language-Action Model for Synergizing Cognition and Action in Robotic Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2411.19650-b31b1b.svg)](https://arxiv.org/abs/2411.19650) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://cogact.github.io)

- **RoboVLMs**, Towards Generalist Robot Policies: What Matters in Building Vision-Language-Action Models. [![arXiv](https://img.shields.io/badge/arXiv-2412.14058-b31b1b.svg)](https://arxiv.org/abs/2412.14058) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://robovlms.github.io)

- [⭐️] **π0**, π0: A Vision-Language-Action Flow Model for General Robot Control. [![arXiv](https://img.shields.io/badge/arXiv-2410.24164-b31b1b.svg)](https://arxiv.org/abs/2410.24164) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://www.pi.website/blog/pi0)

- [⭐️] **OpenVLA**, OpenVLA: An Open-Source Vision-Language-Action Model. [![arXiv](https://img.shields.io/badge/arXiv-2406.09246-b31b1b.svg)](https://arxiv.org/abs/2406.09246) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://openvla.github.io)

- **RoboFlamingo**, Vision-Language Foundation Models as Effective Robot Imitators. [![arXiv](https://img.shields.io/badge/arXiv-2311.01378-b31b1b.svg)](https://arxiv.org/abs/2311.01378) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://roboflamingo.github.io)

- [⭐️] **RT-2**, RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control. [![arXiv](https://img.shields.io/badge/arXiv-2307.15818-b31b1b.svg)](https://arxiv.org/abs/2307.15818) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://robotics-transformer2.github.io)


## World Action Models in VLA

- [⭐️] **Cosmos Policy**, Cosmos Policy: Fine-Tuning Video Models for Visuomotor Control and Planning. [![arXiv](https://img.shields.io/badge/arXiv-2601.16163-b31b1b.svg)](https://arxiv.org/abs/2601.16163) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://research.nvidia.com/labs/dir/cosmos-policy/)

- **MM-ACT**, MM-ACT: Learn from Multimodal Parallel Generation to Act. [![arXiv](https://img.shields.io/badge/arXiv-2512.00975-b31b1b.svg)](https://arxiv.org/abs/2512.00975) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/HHYHRHY/MM-ACT)

- **RynnVLA-002**, RynnVLA-002: A Unified Vision-Language-Action and World Model. [![arXiv](https://img.shields.io/badge/arXiv-2511.17502-b31b1b.svg)](https://arxiv.org/abs/2511.17502) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/alibaba-damo-academy/RynnVLA-002)

- **F1**, F1: A Vision-Language-Action Model Bridging Understanding and Generation to Actions. [![arXiv](https://img.shields.io/badge/arXiv-2509.06951-b31b1b.svg)](https://arxiv.org/abs/2509.06951) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://aopolin-lv.github.io/F1-VLA/)

- **FlowVLA**, FlowVLA: Visual Chain of Thought-based Motion Reasoning for Vision-Language-Action Models. [![arXiv](https://img.shields.io/badge/arXiv-2508.18269-b31b1b.svg)](https://arxiv.org/abs/2508.18269) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://irpn-lab.github.io/FlowVLA/)

- [⭐️] **DreamVLA**, DreamVLA: A Vision-Language-Action Model Dreamed with Comprehensive World Knowledge. [![arXiv](https://img.shields.io/badge/arXiv-2507.04447-b31b1b.svg)](https://arxiv.org/abs/2507.04447) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://zhangwenyao1.github.io/DreamVLA/)

- [⭐️] **WorldVLA**, WorldVLA: Towards Autoregressive Action World Model. [![arXiv](https://img.shields.io/badge/arXiv-2506.21539-b31b1b.svg)](https://arxiv.org/abs/2506.21539) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/alibaba-damo-academy/RynnVLA-002)

- **CoT-VLA**, CoT-VLA: Visual Chain-of-Thought Reasoning for Vision-Language-Action Models. [![arXiv](https://img.shields.io/badge/arXiv-2503.22020-b31b1b.svg)](https://arxiv.org/abs/2503.22020) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://cot-vla.github.io)

- [⭐️] **UP-VLA**, UP-VLA: A Unified Understanding and Prediction Model for Embodied Agent. [![arXiv](https://img.shields.io/badge/arXiv-2501.18867-b31b1b.svg)](https://arxiv.org/abs/2501.18867) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/CladernyJorn/UP-VLA)

## VLA with Understanding and Reasoning

- **MolmoAct**, MolmoAct: Action Reasoning Models that can Reason in Space. [![arXiv](https://img.shields.io/badge/arXiv-2508.07917-b31b1b.svg)](https://arxiv.org/abs/2508.07917) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://allenai.org/blog/molmoact)

- [⭐️] **π0.5**, π0.5: a Vision-Language-Action Model with Open-World Generalization. [![arXiv](https://img.shields.io/badge/arXiv-2504.16054-b31b1b.svg)](https://arxiv.org/abs/2504.16054) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://www.pi.website/blog/pi05)

- **ChatVLA**, ChatVLA: Unified Multimodal Understanding and Robot Control with Vision-Language-Action Model. [![arXiv](https://img.shields.io/badge/arXiv-2502.14420-b31b1b.svg)](https://arxiv.org/abs/2502.14420) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://chatvla.github.io)

## VLA with 3D/4D Modelling

- **4D-VLA**, 4D-VLA: Spatiotemporal Vision-Language-Action Pretraining with Cross-Scene Calibration. [![arXiv](https://img.shields.io/badge/arXiv-2506.22242-b31b1b.svg)](https://arxiv.org/abs/2506.22242) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/LogosRoboticsGroup/4D-VLA)

- **3D CAVLA**, 3D CAVLA: Leveraging Depth and 3D Context to Generalize Vision Language Action Models for Unseen Tasks. [![arXiv](https://img.shields.io/badge/arXiv-2505.05800-b31b1b.svg)](https://arxiv.org/abs/2505.05800) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://3d-cavla.github.io)

- **SpatialVLA**, SpatialVLA: Exploring Spatial Representations for Visual-Language-Action Model. [![arXiv](https://img.shields.io/badge/arXiv-2501.15830-b31b1b.svg)](https://arxiv.org/abs/2501.15830) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://spatialvla.github.io)

- [⭐️] **3D-VLA**, 3D-VLA: A 3D Vision-Language-Action Generative World Model. [![arXiv](https://img.shields.io/badge/arXiv-2403.09631-b31b1b.svg)](https://arxiv.org/abs/2403.09631) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/UMass-Embodied-AGI/3D-VLA)


## VLA with Reinforcement Learning

- **EVOLVE-VLA**, EVOLVE-VLA: Test-Time Training from Environment Feedback for Vision-Language-Action Models. [![arXiv](https://img.shields.io/badge/arXiv-2512.14666-b31b1b.svg)](https://arxiv.org/abs/2512.14666)[![Website](https://img.shields.io/badge/Website-Link-blue)](https://showlab.github.io/EVOLVE-VLA/)

- **AVA-VLA**, AVA-VLA: Improving Vision-Language-Action models with Active Visual Attention. [![arXiv](https://img.shields.io/badge/arXiv-2511.18960-b31b1b.svg)](https://arxiv.org/abs/2511.18960)

- **SRPO**, SRPO: Self-Referential Policy Optimization for Vision-Language-Action Models. [![arXiv](https://img.shields.io/badge/arXiv-2511.15605-b31b1b.svg)](https://arxiv.org/abs/2511.15605)

- **World-Env**, World-Env: Leveraging World Model as a Virtual Environment for VLA Post-Training. [![arXiv](https://img.shields.io/badge/arXiv-2509.24948-b31b1b.svg)](https://arxiv.org/abs/2509.24948)[![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/amap-cvlab/world-env)

- **SimpleVLA-RL**, SimpleVLA-RL: Scaling VLA Training via Reinforcement Learning. [![arXiv](https://img.shields.io/badge/arXiv-2509.09674-b31b1b.svg)](https://arxiv.org/abs/2509.09674)[![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/PRIME-RL/SimpleVLA-RL)

- **VLA-Reasoner**, VLA-Reasoner: Empowering Vision-Language-Action Models with Reasoning via Online Monte Carlo Tree Search. [![arXiv](https://img.shields.io/badge/arXiv-2509.22643-b31b1b.svg)](https://arxiv.org/abs/2509.22643)

- [⭐️] **ThinkAct**, ThinkAct: Vision-Language-Action Reasoning via Reinforced Visual Latent Planning. [![arXiv](https://img.shields.io/badge/arXiv-2507.16815-b31b1b.svg)](https://arxiv.org/abs/2507.16815)[![Website](https://img.shields.io/badge/Website-Link-blue)](https://jasper0314-huang.github.io/thinkact-vla/)

- **TGRPO**, TGRPO :Fine-tuning Vision-Language-Action Model via Trajectory-wise Group Relative Policy Optimization. [![arXiv](https://img.shields.io/badge/arXiv-2506.08440-b31b1b.svg)](https://arxiv.org/abs/2506.08440)

- **VLA-RL**, VLA-RL: Towards Masterful and General Robotic Manipulation with Scalable Reinforcement Learning. [![arXiv](https://img.shields.io/badge/arXiv-2505.18719-b31b1b.svg)](https://arxiv.org/abs/2505.18719)[![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/GuanxingLu/vlarl)

- **RIPT-VLA**, Interactive Post-Training for Vision-Language-Action Models. [![arXiv](https://img.shields.io/badge/arXiv-2505.17016-b31b1b.svg)](https://arxiv.org/abs/2505.17016)[![Website](https://img.shields.io/badge/Website-Link-blue)](https://ariostgx.github.io/ript_vla/)

- **GRAPE**, GRAPE: Generalizing Robot Policy via Preference Alignment. [![arXiv](https://img.shields.io/badge/arXiv-2411.19309-b31b1b.svg)](https://arxiv.org/abs/2411.19309)[![Website](https://img.shields.io/badge/Website-Link-blue)](https://grape-vla.github.io)


## Efficient VLA

- **MergeVLA**, MergeVLA: Cross-Skill Model Merging Toward a Generalist Vision-Language-Action Agent. [![arXiv](https://img.shields.io/badge/arXiv-2511.18810-b31b1b.svg)](https://arxiv.org/abs/2511.18810) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://mergevla.github.io)

- **VLA-Adapter**, VLA-Adapter: An Effective Paradigm for Tiny-Scale Vision-Language-Action Model. [![arXiv](https://img.shields.io/badge/arXiv-2509.09372-b31b1b.svg)](https://arxiv.org/abs/2509.09372) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://vla-adapter.github.io)

- **FLOWER**, FLOWER: Democratizing Generalist Robot Policies with Efficient Vision-Language-Action Flow Policies. [![arXiv](https://img.shields.io/badge/arXiv-2509.04996-b31b1b.svg)](https://arxiv.org/abs/2509.04996) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://intuitive-robots.github.io/flower_vla/)

- [⭐️] **TinyVLA**, TinyVLA: Towards Fast, Data-Efficient Vision-Language-Action Models for Robotic Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2409.12514-b31b1b.svg)](https://arxiv.org/abs/2409.12514) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://tiny-vla.github.io)


## VLA with Latent Actions

- **Motus**, Motus: A Unified Latent Action World Model. [![arXiv](https://img.shields.io/badge/arXiv-2512.13030-b31b1b.svg)](https://arxiv.org/abs/2512.13030) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://motus-robotics.github.io/motus)

- [⭐️] **GR00T N1**, GR00T N1: An Open Foundation Model for Generalist Humanoid Robots. [![arXiv](https://img.shields.io/badge/arXiv-2503.14734-b31b1b.svg)](https://arxiv.org/abs/2503.14734) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://developer.nvidia.com/isaac/gr00t)

- [⭐️] **LAPA**, Latent Action Pretraining from Videos. [![arXiv](https://img.shields.io/badge/arXiv-2410.11758-b31b1b.svg)](https://arxiv.org/abs/2410.11758) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://latentactionpretraining.github.io)


## Domain-Specific VLA (e.g., Humanoid, Tactile)

- **Tactile-VLA**, Tactile-VLA: Unlocking Vision-Language-Action Model's Physical Knowledge for Tactile Generalization. [![arXiv](https://img.shields.io/badge/arXiv-2507.09160-b31b1b.svg)](https://arxiv.org/abs/2507.09160)[![Website](https://img.shields.io/badge/Website-Link-blue)](https://jialeihuang.github.io/tactileVLA.github.io/)

- [⭐️] **GR00T N1**, GR00T N1: An Open Foundation Model for Generalist Humanoid Robots. [![arXiv](https://img.shields.io/badge/arXiv-2503.14734-b31b1b.svg)](https://arxiv.org/abs/2503.14734) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://developer.nvidia.com/isaac/gr00t)

- **CombatVLA**, CombatVLA: An Efficient Vision-Language-Action Model for Combat Tasks in 3D Action Role-Playing Games. [![arXiv](https://img.shields.io/badge/arXiv-2503.09527-b31b1b.svg)](https://arxiv.org/abs/2503.09527) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://combatvla.github.io)

- **Humanoid-VLA**, Humanoid-VLA: Towards Universal Humanoid Control with Visual Integration. [![arXiv](https://img.shields.io/badge/arXiv-2502.14795-b31b1b.svg)](https://arxiv.org/abs/2502.14795)

## Other Topics in VLA

- **DynamicVLA**, DynamicVLA: A Vision-Language-Action Model for Dynamic Object Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2601.22153-b31b1b.svg)](https://arxiv.org/abs/2601.22153) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/hzxie/DynamicVLA)

- **MemoryVLA**, MemoryVLA: Perceptual-Cognitive Memory in Vision-Language-Action Models for Robotic Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2508.19236-b31b1b.svg)](https://arxiv.org/abs/2508.19236) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://shihao1895.github.io/MemoryVLA/)

- **ReconVLA**, ReconVLA: Reconstructive Vision-Language-Action Model as Effective Robot Perceiver. [![arXiv](https://img.shields.io/badge/arXiv-2508.10333-b31b1b.svg)](https://arxiv.org/abs/2508.10333) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://zionchow.github.io/ReconVLA/)

- **TraceVLA**, TraceVLA: Visual Trace Prompting Enhances Spatial-Temporal Awareness for Generalist Robotic Policies. [![arXiv](https://img.shields.io/badge/arXiv-2412.10345-b31b1b.svg)](https://arxiv.org/abs/2412.10345) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://tracevla.github.io)


## Traditional Policies

- **State-free Policy**, Do You Need Proprioceptive States in Visuomotor Policies?. [![arXiv](https://img.shields.io/badge/arXiv-2509.18644-b31b1b.svg)](https://arxiv.org/abs/2509.18644) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://statefreepolicy.github.io)

- [⭐️] **UVAM**, Unified Video Action Model. [![arXiv](https://img.shields.io/badge/arXiv-2503.00200-b31b1b.svg)](https://arxiv.org/abs/2503.00200) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://unified-video-action-model.github.io)

- **Seer**, Predictive Inverse Dynamics Models are Scalable Learners for Robotic Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2412.15109-b31b1b.svg)](https://arxiv.org/abs/2412.15109) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/InternRobotics/Seer)

- **GR-2**, GR-2: A Generative Video-Language-Action Model with Web-Scale Knowledge for Robot Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2410.06158-b31b1b.svg)](https://arxiv.org/abs/2410.06158) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://gr2-manipulation.github.io)

- [⭐️] **RDT-1B**, RDT-1B: a Diffusion Foundation Model for Bimanual Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2410.07864-b31b1b.svg)](https://arxiv.org/abs/2410.07864) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://rdt-robotics.github.io/rdt-robotics/)

- **ReKep**, ReKep: Spatio-Temporal Reasoning of Relational Keypoint Constraints for Robotic Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2409.01652-b31b1b.svg)](https://arxiv.org/abs/2409.01652) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://rekep-robot.github.io)

- **HPT**, Scaling Proprioceptive-Visual Learning with Heterogeneous Pre-trained Transformers. [![arXiv](https://img.shields.io/badge/arXiv-2409.20537-b31b1b.svg)](https://arxiv.org/abs/2409.20537) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://liruiw.github.io/hpt/)

- **MDT**, Multimodal Diffusion Transformer: Learning Versatile Behavior from Multimodal Goals. [![arXiv](https://img.shields.io/badge/arXiv-2407.05996-b31b1b.svg)](https://arxiv.org/abs/2407.05996) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://intuitive-robots.github.io/mdt_policy/)


- [⭐️] **Octo**, Octo: An Open-Source Generalist Robot Policy. [![arXiv](https://img.shields.io/badge/arXiv-2405.12213-b31b1b.svg)](https://arxiv.org/abs/2405.12213) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://octo-models.github.io)

- **ManiGaussian**, ManiGaussian: Dynamic Gaussian Splatting for Multi-task Robotic Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2403.08321-b31b1b.svg)](https://arxiv.org/abs/2403.08321) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://guanxinglu.github.io/ManiGaussian/)

- [⭐️] **DP3**, 3D Diffusion Policy: Generalizable Visuomotor Policy Learning via Simple 3D Representations. [![arXiv](https://img.shields.io/badge/arXiv-2403.03954-b31b1b.svg)](https://arxiv.org/abs/2403.03954) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://3d-diffusion-policy.github.io)

- [⭐️] **GR-1**, Unleashing Large-Scale Video Generative Pre-training for Visual Robot Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2312.13139-b31b1b.svg)](https://arxiv.org/abs/2312.13139) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://gr1-manipulation.github.io)

- [⭐️] **VoxPoser**, VoxPoser: Composable 3D Value Maps for Robotic Manipulation with Language Models. [![arXiv](https://img.shields.io/badge/arXiv-2307.05973-b31b1b.svg)](https://arxiv.org/abs/2307.05973) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://voxposer.github.io)

- **RPT**, Robot Learning with Sensorimotor Pre-training. [![arXiv](https://img.shields.io/badge/arXiv-2306.10007-b31b1b.svg)](https://arxiv.org/abs/2306.10007) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://robotic-pretrained-transformer.github.io)


- [⭐️] **Diffusion Policy**, Diffusion Policy: Visuomotor Policy Learning via Action Diffusion. [![arXiv](https://img.shields.io/badge/arXiv-2303.04137-b31b1b.svg)](https://arxiv.org/abs/2303.04137) [![Website](https://img.shields.io/badge/Website-Link-blue)](http://diffusion-policy.cs.columbia.edu)

- **UniPi**, Learning Universal Policies via Text-Guided Video Generation. [![arXiv](https://img.shields.io/badge/arXiv-2302.00111-b31b1b.svg)](https://arxiv.org/abs/2302.00111) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://universal-policy.github.io/unipi/)

- [⭐️] **RT-1**, RT-1: Robotics Transformer for Real-World Control at Scale. [![arXiv](https://img.shields.io/badge/arXiv-2212.06817-b31b1b.svg)](https://arxiv.org/abs/2212.06817) [![Website](https://img.shields.io/badge/Website-Link-blue)](http://robotics-transformer1.github.io)

- [⭐️] **PerAct**, Perceiver-Actor: A Multi-Task Transformer for Robotic Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2209.05451-b31b1b.svg)](https://arxiv.org/abs/2209.05451) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://peract.github.io)

- **DayDreamer**, DayDreamer: World Models for Physical Robot Learning. [![arXiv](https://img.shields.io/badge/arXiv-2206.14176-b31b1b.svg)](https://arxiv.org/abs/2206.14176) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://danijar.com/project/daydreamer/)

- [⭐️] **Diffusers**, Planning with Diffusion for Flexible Behavior Synthesis. [![arXiv](https://img.shields.io/badge/arXiv-2205.09991-b31b1b.svg)](https://arxiv.org/abs/2205.09991) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://diffusion-planning.github.io)

- [⭐️] **Zero-Shot Planner**, Language Models as Zero-Shot Planners: Extracting Actionable Knowledge for Embodied Agents. [![arXiv](https://img.shields.io/badge/arXiv-2201.07207-b31b1b.svg)](https://arxiv.org/abs/2201.07207) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://wenlonghuang.com/language-planner/)


## Datasets

- [⭐️] **DROID**, DROID: A Large-Scale In-The-Wild Robot Manipulation Dataset. [![arXiv](https://img.shields.io/badge/arXiv-2403.12945-b31b1b.svg)](https://arxiv.org/abs/2403.12945) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://droid-dataset.github.io)

- [⭐️] **Open X-Embodiment**, Open X-Embodiment: Robotic Learning Datasets and RT-X Models. [![arXiv](https://img.shields.io/badge/arXiv-2310.08864-b31b1b.svg)](https://arxiv.org/abs/2310.08864) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://robotics-transformer-x.github.io)


## Benchmark / Environment
- **LIBERO-Plus**, LIBERO-Plus: In-depth Robustness Analysis of Vision-Language-Action Models [![arXiv](https://img.shields.io/badge/arXiv-2510.13626-b31b1b.svg)](https://arxiv.org/abs/2510.13626) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://sylvestf.github.io/LIBERO-plus/)

- [⭐️] **RoboTwin 2.0**, RoboTwin 2.0: A Scalable Data Generator and Benchmark with Strong Domain Randomization for Robust Bimanual Robotic Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2506.18088-b31b1b.svg)](https://arxiv.org/abs/2506.18088) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/robotwin-Platform/robotwin/)

- **RoboCasa**, RoboCasa: Large-Scale Simulation of Everyday Tasks for Generalist Robots. [![arXiv](https://img.shields.io/badge/arXiv-2406.02523-b31b1b.svg)](https://arxiv.org/abs/2406.02523) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://robocasa.ai)

- **SimplerEnv**, Evaluating Real-World Robot Manipulation Policies in Simulation. [![arXiv](https://img.shields.io/badge/arXiv-2405.05941-b31b1b.svg)](https://arxiv.org/abs/2405.05941) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://simpler-env.github.io)

- [⭐️] **LIBERO**, LIBERO: Benchmarking Knowledge Transfer for Lifelong Robot Learning. [![arXiv](https://img.shields.io/badge/arXiv-2306.03310-b31b1b.svg)](https://arxiv.org/abs/2306.03310) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://libero-project.github.io/main.html)

- **FurnitureBench**, FurnitureBench: Reproducible Real-World Benchmark for Long-Horizon Complex Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2305.12821-b31b1b.svg)](https://arxiv.org/abs/2305.12821) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://clvrai.github.io/furniture-bench/)

- [⭐️] **CALVIN**, CALVIN: A Benchmark for Language-Conditioned Policy Learning for Long-Horizon Robot Manipulation Tasks. [![arXiv](https://img.shields.io/badge/arXiv-2112.03227-b31b1b.svg)](https://arxiv.org/abs/2112.03227) [![Website](https://img.shields.io/badge/Website-Link-blue)](http://calvin.cs.uni-freiburg.de)

- [⭐️] **SAPIEN**, SAPIEN: A SimulAted Part-based Interactive ENvironment. [![arXiv](https://img.shields.io/badge/arXiv-2003.08515-b31b1b.svg)](https://arxiv.org/abs/2003.08515) (https://sapien.ucsd.edu)

- [⭐️] **RLBench**, RLBench: The Robot Learning Benchmark & Learning Environment.[![arXiv](https://img.shields.io/badge/arXiv-1909.12271-b31b1b.svg)](https://arxiv.org/abs/1909.12271) [![Website](https://img.shields.io/badge/Website-Link-blue)] [![Website](https://img.shields.io/badge/Website-Link-blue)](https://sites.google.com/view/rlbench)

## Physics Engine

- [⭐️] **Cosmos (neural engine)**, Cosmos World Foundation Model Platform for Physical AI  [![arXiv](https://img.shields.io/badge/arXiv-2501.03575-b31b1b.svg)](https://arxiv.org/abs/2501.03575) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/nvidia-cosmos/cosmos-predict1)

- [⭐️] **PhysX**, [![Website](https://img.shields.io/badge/Website-Link-blue)](https://developer.nvidia.com/physx-sdk)

- [⭐️] **MuJoCo**. [![Website](https://img.shields.io/badge/Website-Link-blue)](https://mujoco.org)

- [⭐️] **PyBullet**. [![Website](https://img.shields.io/badge/Website-Link-blue)](https://pybullet.org/wordpress/)

## Hardware

- **GELLO**, GELLO: A General, Low-Cost, and Intuitive Teleoperation Framework for Robot Manipulators. [![arXiv](https://img.shields.io/badge/arXiv-2309.13037-b31b1b.svg)](https://arxiv.org/abs/2309.13037) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://wuphilipp.github.io/gello_site/)

- [⭐️] **ALOHA**, Learning Fine-Grained Bimanual Manipulation with Low-Cost Hardware. [![arXiv](https://img.shields.io/badge/arXiv-2304.13705-b31b1b.svg)](https://arxiv.org/abs/2304.13705) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://tonyzhaozh.github.io/aloha/)

## Acknowledgements
Thanks to [Awesome World Models](https://github.com/knightnemo/Awesome-World-Models/tree/main) for the template.



