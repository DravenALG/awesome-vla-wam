<div align="center">

# 🤖 Awesome VLA & WAM

**📜 A Curated List of Vision-Language-Action (VLA) and World Action Models (WAM) Research and Beyond** </br>

<p align="center">
  <img src="awesome-vla-wam.jpg" alt="Awesome VLA & WAM" width="100%" style="border-radius: 15px; box-shadow: 0 4px 24px rgba(0,0,0,.1); margin: 5px 0;">
</p>

*Photo Credit: [Gemini-Nano-Banana🍌](https://aistudio.google.com/models/gemini-3-pro-image)*.

</div>

## Overview
- 🎯 [Aim](#aim)
- 📚 [VLA Definition](#vla-definition) | [WAM Definition](#wam-definition) | [Policy Definition](#policy-definition) | [LAM Definition](#lam-definition) | [HAP Definition](#hap-definition) | [CaP Definition](#cap-definition)

**Vision-Language-Action (VLA) Models**
- 🧠 [VLA Models](#vla-models)

**World Action Models (WAM)**
- 🌌 [World Models](#world-models)
- 🌍 [World Action Models](#world-action-models)

**Policies**
- 🦾 [Policies](#policies)

**Latent Action Models (LAM)**
- 🧭 [Latent Action Models](#latent-action-models)

**Human Action Pretraining (HAP)**
- 💪 [Human Action Pretraining](#human-action-pretraining)

**Code as Policy (CaP)**
- 🌐 [Code as Policy](#code-as-policy)

**Resources**
- 🔍 [Survey](#survey)
- 💾 [Robotics Datasets](#robotics-datasets)
- 👨🏻 [Ego Human Datasets](#ego-human-datasets)
- 📊 [Benchmark / Environment](#benchmark--environment)
- 🏞️ [Physics Engine](#physics-engine)
- 🧑‍💻 [Software](#software)
- 🖥️ [Hardware](#hardware)


## Aim
This repository provides a curated and systematically organized collection of research on Vision-Language-Action models (VLAs), World Action Models (WAMs), and related approaches. It aims to offer a comprehensive view of recent advances toward robotics foundation models and to clarify the connections among different research directions.

The repository will be continuously updated and refined as the field evolves. Contributions are highly welcome! If you know of relevant papers that should be included, please submit a pull request or open an issue. Join us in maintaining a high-quality VLA, WAM & More research list and advancing the development of robotics foundation models.


## VLA Definition
Vision-Language-Action models (VLAs) are robot policies built upon pretrained Vision-Language Models (VLMs). By inheriting their rich visual understanding, language grounding, and semantic knowledge, VLAs provide a scalable path toward general-purpose, language-conditioned robot policies. The term Vision-Language-Action model was introduced and formally established by RT-2.

- [⭐️] **RT-2**, RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control. [![arXiv](https://img.shields.io/badge/arXiv-2307.15818-b31b1b.svg)](https://arxiv.org/abs/2307.15818) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://robotics-transformer2.github.io)

## WAM Definition
World Action Models (WAMs) are robot policies that explicitly leverage world modeling—i.e., predicting future states or representations of the environment—to support or jointly perform action prediction. The term World Action Model was formally coined by DreamZero.

- [⭐️] **DreamZero**, World Action Models are Zero-shot Policies. [![arXiv](https://img.shields.io/badge/arXiv-2602.15922-b31b1b.svg)](https://arxiv.org/abs/2602.15922) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://dreamzero0.github.io)

VLAs and WAMs are not mutually exclusive. A WAM built upon a pretrained VLM can simultaneously be considered both a VLA and a WAM.

## Policy Definition

In its broadest sense, a robot policy refers to any model that predicts actions, including VLAs and WAMs. In this repository, however, the Policy category specifically refers to robot policies trained primarily from scratch on robot data for action prediction, without relying on pretrained VLMs or explicit visual (2D/Video/3D) generation pretraining. A representative example is Diffusion Policy.

- [⭐️] **Diffusion Policy**, Diffusion Policy: Visuomotor Policy Learning via Action Diffusion. [![arXiv](https://img.shields.io/badge/arXiv-2303.04137-b31b1b.svg)](https://arxiv.org/abs/2303.04137) [![Website](https://img.shields.io/badge/Website-Link-blue)](http://diffusion-policy.cs.columbia.edu)

## LAM Definition

Latent Action Models (LAMs) learn action-like latent representations from unlabeled videos or observation sequences. These latent actions capture the transitions between states and can serve as supervision for policy pretraining. The pretrained model is subsequently finetuned to predict executable robot actions using labeled robot data. A representative example is LAPA.

- [⭐️] **LAPA**, Latent Action Pretraining from Videos. [![arXiv](https://img.shields.io/badge/arXiv-2410.11758-b31b1b.svg)](https://arxiv.org/abs/2410.11758) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://latentactionpretraining.github.io)

## HAP Definition

Human Action Pretraining (HAP) methods pretrain robot policies on human behavior data using explicit action supervision extracted or recorded from human demonstrations, such as hand pose, full-body trajectories or UMI pose. The pretrained policy is subsequently aligned or finetuned on robot data to produce executable robot actions. A representative example is EgoScale.

- [⭐️] **Egoscale**, EgoScale: Scaling Dexterous Manipulation with Diverse Egocentric Human Data. [![arXiv](https://img.shields.io/badge/arXiv-2602.16710-b31b1b.svg)](https://arxiv.org/abs/2602.16710) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://research.nvidia.com/labs/gear/egoscale/)


## CaP Definition

Code-as-Policy (CaP) methods use Large Language Models (LLMs) agentic system as high-level planners to generate executable programs that compose perception modules and low-level robot policys (traditional control API or policy models) for embodied task execution. This concept was introduced by Code as Policies.

- [⭐️] **Code as Policies**, Code as Policies: Language Model Programs for Embodied Control. [![arXiv](https://img.shields.io/badge/arXiv-2209.07753-b31b1b.svg)](https://arxiv.org/abs/2209.07753) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://code-as-policies.github.io)

## VLA Models

- [⭐️] **Gemini Robotics 2**, Gemini Robotics 2: The intelligence layer to power any kind of robot. [![Website](https://img.shields.io/badge/Website-Link-blue)](https://deepmind.google/models/gemini-robotics/)

- [⭐️] **Xiaomi-Robotics-1**, Xiaomi-Robotics-1: Scaling Vision-Language-Action Models with over 100K Hours of Real-World Trajectories. [![arXiv](https://img.shields.io/badge/arXiv-2607.15330-b31b1b.svg)](https://arxiv.org/abs/2607.15330) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://robotics.xiaomi.com/xiaomi-robotics-1.html)

- [⭐️] **Qwen-RobotManip**, Qwen-RobotManip Technical Report: Alignment Unlocks Scale for Robotic Manipulation Foundation Models. [![arXiv](https://img.shields.io/badge/arXiv-2606.17846-b31b1b.svg)](https://arxiv.org/abs/2606.17846) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://qwen.ai/blog?id=qwen-robotmanip)

- **FOCA-VLA** FOCA: Future-Oriented Conditioning for Data-Efficient Vision-Language-Action Adaptation. [![arXiv](https://img.shields.io/badge/arXiv-2606.20867-b31b1b.svg)](https://arxiv.org/abs/2606.20867) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://focavla.github.io/)

- **Qwen-VLA**, Qwen-VLA: Unifying Vision-Language-Action Modeling across Tasks, Environments, and Robot Embodiments. [![arXiv](https://img.shields.io/badge/arXiv-2605.30280-b31b1b.svg)](https://arxiv.org/abs/2605.30280) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://qwen.ai/blog?id=qwenvla)

- **Pion**, Rethinking Muon Beyond Pretraining: Spectral Failures and High-Pass Remedies for VLA and RLVR. [![arXiv](https://img.shields.io/badge/arXiv-2605.19282-b31b1b.svg)](https://arxiv.org/abs/2605.19282) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://chongyu-fan.netlify.app/posts/pion/)

- [⭐️] **MolmoAct2**, MolmoAct2 Action Reasoning Models for Real-World Deployment. [![arXiv](https://img.shields.io/badge/arXiv-2605.02881-b31b1b.svg)](https://arxiv.org/abs/2605.02881) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://allenai.org/blog/molmoact2)

- **RLDX-1**, RLDX-1 Technical Report. [![arXiv](https://img.shields.io/badge/arXiv-2605.03269-b31b1b.svg)](https://arxiv.org/abs/2605.03269) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://www.rlwrld.ai/en/rldx-1)

- **GridS**, See What Matters: Differentiable Grid Sample Pruning for Generalizable Vision-Language-Action Model. [![arXiv](https://img.shields.io/badge/arXiv-2605.11817-b31b1b.svg)](https://arxiv.org/abs/2605.11817) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/Fediory/Grid-Sampler)

- [⭐️] **π0.7**, π0.7: a Steerable Generalist Robotic Foundation Model with Emergent Capabilities. [![arXiv](https://img.shields.io/badge/arXiv-2604.15483-b31b1b.svg)](https://arxiv.org/abs/2604.15483) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://www.pi.website/blog/pi07)

- **PokeVLA**, PokeVLA: Empowering Pocket-Sized Vision-Language-Action Model with Comprehensive World Knowledge Guidance. [![arXiv](https://img.shields.io/badge/arXiv-2604.20834-b31b1b.svg)](https://arxiv.org/abs/2604.20834) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://getterupper.github.io/PokeVLA)

- **LaST-R1**, LaST-R1: Reinforcing Robotic Manipulation via Adaptive Physical Latent Reasoning. [![arXiv](https://img.shields.io/badge/arXiv-2604.28192-b31b1b.svg)](https://arxiv.org/abs/2604.28192)[![Website](https://img.shields.io/badge/Website-Link-blue)](https://siriyep.github.io/last-r1/)

- **StarVLA-α**, StarVLA-α: Reducing Complexity in Vision-Language-Action Systems. [![arXiv](https://img.shields.io/badge/arXiv-2604.11757-b31b1b.svg)](https://arxiv.org/abs/2604.11757) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/starVLA/starVLA)

- **StarVLA**, StarVLA: A Lego-like Codebase for Vision-Language-Action Model Developing. [![arXiv](https://img.shields.io/badge/arXiv-2604.05014-b31b1b.svg)](https://arxiv.org/abs/2604.05014) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/starVLA/starVLA)

- **DIAL** DIAL: Decoupling Intent and Action via Latent World Modeling for End-to-End VLA. [![arXiv](https://img.shields.io/badge/arXiv-2603.29844-b31b1b.svg)](https://arxiv.org/abs/2603.29844) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://xpeng-robotics.github.io/dial/)

- [⭐️] **VLANeXt**, VLANeXt: Recipes for Building Strong VLA Models. [![arXiv](https://img.shields.io/badge/arXiv-2602.18532-b31b1b.svg)](https://arxiv.org/abs/2602.18532) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://dravenalg.github.io/VLANeXt/)

- **LAP**, LAP: Language-Action Pre-Training Enables Zero-shot Cross-Embodiment Transfer. [![arXiv](https://img.shields.io/badge/arXiv-2602.10556-b31b1b.svg)](https://arxiv.org/abs/2602.10556) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://lap-vla.github.io)

- **HBVLA**, HBVLA: Pushing 1-Bit Post-Training Quantization for Vision-Language-Action Models. [![arXiv](https://img.shields.io/badge/arXiv-2602.13710-b31b1b.svg)](https://arxiv.org/abs/2602.13710)

- **CoVer-VLA**, Scaling Verification Can Be More Effective than Scaling Policy Learning for Vision-Language-Action Alignment. [![arXiv](https://img.shields.io/badge/arXiv-2602.12281-b31b1b.svg)](https://arxiv.org/abs/2602.12281) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://cover-vla.github.io)

- **HoloBrain-0**, HoloBrain-0 Technical Report. [![arXiv](https://img.shields.io/badge/arXiv-2602.12062-b31b1b.svg)](https://arxiv.org/abs/2602.12062) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://horizonrobotics.github.io/robot_lab/holobrain/)

- **ABot-M0**, ABot-M0: VLA Foundation Model for Robotic Manipulation with Action Manifold Learning. [![arXiv](https://img.shields.io/badge/arXiv-2602.11236-b31b1b.svg)](https://arxiv.org/abs/2602.11236) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://amap-cvlab.github.io/ABot-Manipulation/)

- **SimVLA**, SimVLA: A Simple VLA Baseline for Robotic Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2602.18224-b31b1b.svg)](https://arxiv.org/abs/2602.18224) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://frontierrobo.github.io/SimVLA/)

- **DynamicVLA**, DynamicVLA: A Vision-Language-Action Model for Dynamic Object Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2601.22153-b31b1b.svg)](https://arxiv.org/abs/2601.22153) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/hzxie/DynamicVLA)

- **Lingbot-VLA**, A Pragmatic VLA Foundation Model. [![arXiv](https://img.shields.io/badge/arXiv-2601.18692-b31b1b.svg)](https://arxiv.org/abs/2601.18692) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://technology.robbyant.com/lingbot-vla/)

- **ACoT-VLA**, ACoT-VLA: Action Chain-of-Thought for Vision-Language-Action Models. [![arXiv](https://img.shields.io/badge/arXiv-2601.11404-b31b1b.svg)](https://arxiv.org/abs/2601.11404) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/AgibotTech/ACoT-VLA)

- **EVOLVE-VLA**, EVOLVE-VLA: Test-Time Training from Environment Feedback for Vision-Language-Action Models. [![arXiv](https://img.shields.io/badge/arXiv-2512.14666-b31b1b.svg)](https://arxiv.org/abs/2512.14666)[![Website](https://img.shields.io/badge/Website-Link-blue)](https://showlab.github.io/EVOLVE-VLA/)

- **FASTer**, FASTer: Toward Efficient Autoregressive Vision Language Action Modeling via Neural Action Tokenization. [![arXiv](https://img.shields.io/badge/arXiv-2512.04952-b31b1b.svg)](https://arxiv.org/abs/2512.04952)

- **GenieReasoner**, Unified Embodied VLM Reasoning with Robotic Action via Autoregressive Discretized Pre-training. [![arXiv](https://img.shields.io/badge/arXiv-2512.24125-b31b1b.svg)](https://arxiv.org/abs/2512.24125) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://geniereasoner.github.io/GenieReasoner/)

- [⭐️] **π∗0.6**, π∗0.6: a VLA That Learns From Experience. [![arXiv](https://img.shields.io/badge/arXiv-2511.14759-b31b1b.svg)](https://arxiv.org/abs/2511.14759) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://www.pi.website/blog/pistar06)

- **METIS**, METIS: Multi-Source Egocentric Training for Integrated Dexterous Vision-Language-Action Model. [![arXiv](https://img.shields.io/badge/arXiv-2511.17366-b31b1b.svg)](https://arxiv.org/abs/2511.17366)[![Website](https://img.shields.io/badge/Website-Link-blue)](https://aureleopku.github.io/METIS/)

- **MergeVLA**, MergeVLA: Cross-Skill Model Merging Toward a Generalist Vision-Language-Action Agent. [![arXiv](https://img.shields.io/badge/arXiv-2511.18810-b31b1b.svg)](https://arxiv.org/abs/2511.18810) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://mergevla.github.io)

- **TwinVLA**, TwinVLA: Data-Efficient Bimanual Manipulation with Twin Single-Arm Vision-Language-Action Models. [![arXiv](https://img.shields.io/badge/arXiv-2511.05275-b31b1b.svg)](https://arxiv.org/abs/2511.05275) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://jellyho.github.io/TwinVLA/)

- **SRPO**, SRPO: Self-Referential Policy Optimization for Vision-Language-Action Models. [![arXiv](https://img.shields.io/badge/arXiv-2511.15605-b31b1b.svg)](https://arxiv.org/abs/2511.15605)

- **AVA-VLA**, AVA-VLA: Improving Vision-Language-Action models with Active Visual Attention. [![arXiv](https://img.shields.io/badge/arXiv-2511.18960-b31b1b.svg)](https://arxiv.org/abs/2511.18960)

- **AsyncVLA**, AsyncVLA: Asynchronous Flow Matching for Vision-Language-Action Models. [![arXiv](https://img.shields.io/badge/arXiv-2511.14148-b31b1b.svg)](https://arxiv.org/abs/2511.14148) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/YuhuaJiang2002/AsyncVLA)

- **VLA-0**, VLA-0: Building State-of-the-Art VLAs with Zero Modification. [![arXiv](https://img.shields.io/badge/arXiv-2510.13054-b31b1b.svg)](https://arxiv.org/abs/2510.13054) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://vla0.github.io)

- **X-VLA**, X-VLA: Soft-Prompted Transformer as Scalable Cross-Embodiment Vision-Language-Action Model. [![arXiv](https://img.shields.io/badge/arXiv-2510.10274-b31b1b.svg)](https://arxiv.org/abs/2510.10274) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://thu-air-dream.github.io/X-VLA/)

- **FLOWER**, FLOWER: Democratizing Generalist Robot Policies with Efficient Vision-Language-Action Flow Policies. [![arXiv](https://img.shields.io/badge/arXiv-2509.04996-b31b1b.svg)](https://arxiv.org/abs/2509.04996) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://intuitive-robots.github.io/flower_vla/)

- **VLA-Adapter**, VLA-Adapter: An Effective Paradigm for Tiny-Scale Vision-Language-Action Model. [![arXiv](https://img.shields.io/badge/arXiv-2509.09372-b31b1b.svg)](https://arxiv.org/abs/2509.09372) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://vla-adapter.github.io)

- **SimpleVLA-RL**, SimpleVLA-RL: Scaling VLA Training via Reinforcement Learning. [![arXiv](https://img.shields.io/badge/arXiv-2509.09674-b31b1b.svg)](https://arxiv.org/abs/2509.09674)[![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/PRIME-RL/SimpleVLA-RL)

- **ATE**, Align-Then-stEer: Adapting the Vision-Language Action Models through Unified Latent Guidance. [![arXiv](https://img.shields.io/badge/arXiv-2509.02055-b31b1b.svg)](https://arxiv.org/abs/2509.02055) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://align-then-steer.github.io)

- **VLA-Reasoner**, VLA-Reasoner: Empowering Vision-Language-Action Models with Reasoning via Online Monte Carlo Tree Search. [![arXiv](https://img.shields.io/badge/arXiv-2509.22643-b31b1b.svg)](https://arxiv.org/abs/2509.22643)

- **Discrete Diffusion VLA**, Discrete Diffusion VLA: Bringing Discrete Diffusion to Action Decoding in Vision-Language-Action Policies. [![arXiv](https://img.shields.io/badge/arXiv-2508.20072-b31b1b.svg)](https://arxiv.org/abs/2508.20072) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/Liang-ZX/DiscreteDiffusionVLA/tree/libero)

- **MemoryVLA**, MemoryVLA: Perceptual-Cognitive Memory in Vision-Language-Action Models for Robotic Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2508.19236-b31b1b.svg)](https://arxiv.org/abs/2508.19236) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://shihao1895.github.io/MemoryVLA/)

- **ReconVLA**, ReconVLA: Reconstructive Vision-Language-Action Model as Effective Robot Perceiver. [![arXiv](https://img.shields.io/badge/arXiv-2508.10333-b31b1b.svg)](https://arxiv.org/abs/2508.10333) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://zionchow.github.io/ReconVLA/)

- **MolmoAct**, MolmoAct: Action Reasoning Models that can Reason in Space. [![arXiv](https://img.shields.io/badge/arXiv-2508.07917-b31b1b.svg)](https://arxiv.org/abs/2508.07917) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://allenai.org/blog/molmoact)

- **ThinkAct**, ThinkAct: Vision-Language-Action Reasoning via Reinforced Visual Latent Planning. [![arXiv](https://img.shields.io/badge/arXiv-2507.16815-b31b1b.svg)](https://arxiv.org/abs/2507.16815)[![Website](https://img.shields.io/badge/Website-Link-blue)](https://jasper0314-huang.github.io/thinkact-vla/)

- **Tactile-VLA**, Tactile-VLA: Unlocking Vision-Language-Action Model's Physical Knowledge for Tactile Generalization. [![arXiv](https://img.shields.io/badge/arXiv-2507.09160-b31b1b.svg)](https://arxiv.org/abs/2507.09160)[![Website](https://img.shields.io/badge/Website-Link-blue)](https://jialeihuang.github.io/tactileVLA.github.io/)

- **TGRPO**, TGRPO: Fine-tuning Vision-Language-Action Model via Trajectory-wise Group Relative Policy Optimization. [![arXiv](https://img.shields.io/badge/arXiv-2506.08440-b31b1b.svg)](https://arxiv.org/abs/2506.08440)

- **SmolVLA**, SmolVLA: A Vision-Language-Action Model for Affordable and Efficient Robotics. [![arXiv](https://img.shields.io/badge/arXiv-2506.01844-b31b1b.svg)](https://arxiv.org/abs/2506.01844) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/huggingface/lerobot)

- **4D-VLA**, 4D-VLA: Spatiotemporal Vision-Language-Action Pretraining with Cross-Scene Calibration. [![arXiv](https://img.shields.io/badge/arXiv-2506.22242-b31b1b.svg)](https://arxiv.org/abs/2506.22242) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/LogosRoboticsGroup/4D-VLA)

- **CronusVLA**, CronusVLA: Towards Efficient and Robust Manipulation via Multi-Frame Vision-Language-Action Modeling. [![arXiv](https://img.shields.io/badge/arXiv-2506.19816-b31b1b.svg)](https://arxiv.org/abs/2506.19816) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://lihaohn.github.io/CronusVLA.github.io/)

- **3D CAVLA**, 3D CAVLA: Leveraging Depth and 3D Context to Generalize Vision Language Action Models for Unseen Tasks. [![arXiv](https://img.shields.io/badge/arXiv-2505.05800-b31b1b.svg)](https://arxiv.org/abs/2505.05800) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://3d-cavla.github.io)

- **VLA-RL**, VLA-RL: Towards Masterful and General Robotic Manipulation with Scalable Reinforcement Learning. [![arXiv](https://img.shields.io/badge/arXiv-2505.18719-b31b1b.svg)](https://arxiv.org/abs/2505.18719)[![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/GuanxingLu/vlarl)

- **X-ICM**, Exploring the Limits of Vision-Language-Action Manipulations in Cross-task Generalization. [![arXiv](https://img.shields.io/badge/arXiv-2505.15660-b31b1b.svg)](https://arxiv.org/abs/2505.15660) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://jiaming-zhou.github.io/AGNOSTOS/)

- **RIPT-VLA**, Interactive Post-Training for Vision-Language-Action Models. [![arXiv](https://img.shields.io/badge/arXiv-2505.17016-b31b1b.svg)](https://arxiv.org/abs/2505.17016)[![Website](https://img.shields.io/badge/Website-Link-blue)](https://ariostgx.github.io/ript_vla/)

- **ForceVLA**, ForceVLA: Enhancing VLA Models with a Force-aware MoE for Contact-rich Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2505.22159-b31b1b.svg)](https://arxiv.org/abs/2505.22159) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://sites.google.com/view/forcevla2025)

- [⭐️] **π0.5**, π0.5: a Vision-Language-Action Model with Open-World Generalization. [![arXiv](https://img.shields.io/badge/arXiv-2504.16054-b31b1b.svg)](https://arxiv.org/abs/2504.16054) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://www.pi.website/blog/pi05)

- **NORA**, NORA: A Small Open-Sourced Generalist Vision Language Action Model for Embodied Tasks. [![arXiv](https://img.shields.io/badge/arXiv-2504.19854-b31b1b.svg)](https://arxiv.org/abs/2504.19854) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://declare-lab.github.io/nora)

- [⭐️] **Gemini Robotics**, Gemini Robotics: Bringing AI into the Physical World. [![arXiv](https://img.shields.io/badge/arXiv-2503.20020-b31b1b.svg)](https://arxiv.org/abs/2503.20020) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://deepmind.google/models/gemini-robotics/)

- **CombatVLA**, CombatVLA: An Efficient Vision-Language-Action Model for Combat Tasks in 3D Action Role-Playing Games. [![arXiv](https://img.shields.io/badge/arXiv-2503.09527-b31b1b.svg)](https://arxiv.org/abs/2503.09527) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://combatvla.github.io)

- [⭐️] **OpenVLA-OFT**, Fine-Tuning Vision-Language-Action Models: Optimizing Speed and Success. [![arXiv](https://img.shields.io/badge/arXiv-2502.19645-b31b1b.svg)](https://arxiv.org/abs/2502.19645) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://openvla-oft.github.io)

- **Humanoid-VLA**, Humanoid-VLA: Towards Universal Humanoid Control with Visual Integration. [![arXiv](https://img.shields.io/badge/arXiv-2502.14795-b31b1b.svg)](https://arxiv.org/abs/2502.14795)

- **ChatVLA**, ChatVLA: Unified Multimodal Understanding and Robot Control with Vision-Language-Action Model. [![arXiv](https://img.shields.io/badge/arXiv-2502.14420-b31b1b.svg)](https://arxiv.org/abs/2502.14420) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://chatvla.github.io)

- **SpatialVLA**, SpatialVLA: Exploring Spatial Representations for Visual-Language-Action Model. [![arXiv](https://img.shields.io/badge/arXiv-2501.15830-b31b1b.svg)](https://arxiv.org/abs/2501.15830) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://spatialvla.github.io)

- [⭐️] **FAST**, FAST: Efficient Action Tokenization for Vision-Language-Action Models. [![arXiv](https://img.shields.io/badge/arXiv-2501.09747-b31b1b.svg)](https://arxiv.org/abs/2501.09747) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://www.pi.website/research/fast)


- **TraceVLA**, TraceVLA: Visual Trace Prompting Enhances Spatial-Temporal Awareness for Generalist Robotic Policies. [![arXiv](https://img.shields.io/badge/arXiv-2412.10345-b31b1b.svg)](https://arxiv.org/abs/2412.10345) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://tracevla.github.io)

- **RoboVLMs**, Towards Generalist Robot Policies: What Matters in Building Vision-Language-Action Models. [![arXiv](https://img.shields.io/badge/arXiv-2412.14058-b31b1b.svg)](https://arxiv.org/abs/2412.14058) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://robovlms.github.io)

- **CogACT**, CogACT: A Foundational Vision-Language-Action Model for Synergizing Cognition and Action in Robotic Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2411.19650-b31b1b.svg)](https://arxiv.org/abs/2411.19650) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://cogact.github.io)

- **GRAPE**, GRAPE: Generalizing Robot Policy via Preference Alignment. [![arXiv](https://img.shields.io/badge/arXiv-2411.19309-b31b1b.svg)](https://arxiv.org/abs/2411.19309)[![Website](https://img.shields.io/badge/Website-Link-blue)](https://grape-vla.github.io)

- [⭐️] **π0**, π0: A Vision-Language-Action Flow Model for General Robot Control. [![arXiv](https://img.shields.io/badge/arXiv-2410.24164-b31b1b.svg)](https://arxiv.org/abs/2410.24164) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://www.pi.website/blog/pi0)

- [⭐️] **TinyVLA**, TinyVLA: Towards Fast, Data-Efficient Vision-Language-Action Models for Robotic Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2409.12514-b31b1b.svg)](https://arxiv.org/abs/2409.12514) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://tiny-vla.github.io)

- [⭐️] **OpenVLA**, OpenVLA: An Open-Source Vision-Language-Action Model. [![arXiv](https://img.shields.io/badge/arXiv-2406.09246-b31b1b.svg)](https://arxiv.org/abs/2406.09246) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://openvla.github.io)

- [⭐️] **3D-VLA**, 3D-VLA: A 3D Vision-Language-Action Generative World Model. [![arXiv](https://img.shields.io/badge/arXiv-2403.09631-b31b1b.svg)](https://arxiv.org/abs/2403.09631) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/UMass-Embodied-AGI/3D-VLA)

- **RoboFlamingo**, Vision-Language Foundation Models as Effective Robot Imitators. [![arXiv](https://img.shields.io/badge/arXiv-2311.01378-b31b1b.svg)](https://arxiv.org/abs/2311.01378) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://roboflamingo.github.io)

- [⭐️] **RT-2**, RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control. [![arXiv](https://img.shields.io/badge/arXiv-2307.15818-b31b1b.svg)](https://arxiv.org/abs/2307.15818) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://robotics-transformer2.github.io)

## World Models

- **Qwen-RobotWorld**, Qwen-RobotWorld Technical Report: Unifying Embodied World Modeling through Language-Conditioned Video Generation. [![arXiv](https://img.shields.io/badge/arXiv-2606.17030-b31b1b.svg)](https://arxiv.org/abs/2606.17030) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://qwen.ai/blog?id=qwen-robotworld)

- [⭐️] **Cosmos 3**, Cosmos 3: Omnimodal World Models for Physical AI. [![arXiv](https://img.shields.io/badge/arXiv-2606.02800-b31b1b.svg)](https://arxiv.org/abs/2606.02800) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://research.nvidia.com/labs/cosmos-lab/cosmos3/)

- [⭐️] **DreamDojo**, DreamDojo: A Generalist Robot World Model from Large-Scale Human Videos. [![arXiv](https://img.shields.io/badge/arXiv-2602.06949-b31b1b.svg)](https://arxiv.org/abs/2602.06949) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://dreamdojo-world.github.io)

- **PointWorld**, PointWorld: Scaling 3D World Models for In-The-Wild Robotic Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2601.03782-b31b1b.svg)](https://arxiv.org/abs/2601.03782) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://point-world.github.io)

- **NitroGen**, NitroGen: An Open Foundation Model for Generalist Gaming Agents. [![arXiv](https://img.shields.io/badge/arXiv-2601.02427-b31b1b.svg)](https://arxiv.org/abs/2601.02427) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://nitrogen.minedojo.org)

- **Puffin**, Thinking with Camera: A Unified Multimodal Model for Camera-Centric Understanding and Generation. [![arXiv](https://img.shields.io/badge/arXiv-2510.086735-b31b1b.svg)](https://arxiv.org/abs/2510.086735) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://kangliao929.github.io/projects/puffin/)

- **Yume**, Yume: An Interactive World Generation Model. [![arXiv](https://img.shields.io/badge/arXiv-2507.17744-b31b1b.svg)](https://arxiv.org/abs/2507.17744) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://stdstu12.github.io/YUME-Project/)

- **PlayerOne**, PlayerOne: Egocentric World Simulator. [![arXiv](https://img.shields.io/badge/arXiv-2506.09995-b31b1b.svg)](https://arxiv.org/abs/2506.09995) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://playerone-hku.github.io)

- **Matrix-Game**, Matrix-Game: Interactive World Foundation Model. [![arXiv](https://img.shields.io/badge/arXiv-2506.18701-b31b1b.svg)](https://arxiv.org/abs/2506.18701) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/SkyworkAI/Matrix-Game)

- **WorldMem**, WorldMem: Long-term Consistent World Simulation with Memory. [![arXiv](https://img.shields.io/badge/arXiv-2504.12369-b31b1b.svg)](https://arxiv.org/abs/2504.12369) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://xizaoqu.github.io/worldmem/)

- [⭐️] **Cosmos**, Cosmos World Foundation Model Platform for Physical AI. [![arXiv](https://img.shields.io/badge/arXiv-2501.03575-b31b1b.svg)](https://arxiv.org/abs/2501.03575) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/nvidia-cosmos/cosmos-predict1)

- **GameFactory**, GameFactory: Creating New Games with Generative Interactive Videos. [![arXiv](https://img.shields.io/badge/arXiv-2501.08325-b31b1b.svg)](https://arxiv.org/abs/2501.08325) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://yujiwen.github.io/gamefactory/)

- **The Matrix**, The Matrix: Infinite-Horizon World Generation with Real-Time Moving Control. [![arXiv](https://img.shields.io/badge/arXiv-2412.03568-b31b1b.svg)](https://arxiv.org/abs/2412.03568) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://thematrix1999.github.io)

- [⭐️] **Genie**, Genie: Generative Interactive Environments. [![arXiv](https://img.shields.io/badge/arXiv-2402.15391-b31b1b.svg)](https://arxiv.org/abs/2402.15391) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://sites.google.com/view/genie-2024/)

- **Playable Environments**, Playable Environments: Video Manipulation in Space and Time. [![arXiv](https://img.shields.io/badge/arXiv-2203.01914-b31b1b.svg)](https://arxiv.org/abs/2203.01914)[![Website](https://img.shields.io/badge/Website-Link-blue)](https://willi-menapace.github.io/playable-environments-website/)

- **CADDY**, Playable Video Generation. [![arXiv](https://img.shields.io/badge/arXiv-2101.12195-b31b1b.svg)](https://arxiv.org/abs/2101.12195)[![Website](https://img.shields.io/badge/Website-Link-blue)](https://willi-menapace.github.io/playable-video-generation-website/)

- [⭐️] **ACVP**, Action-Conditional Video Prediction using Deep Networks in Atari Games. [![arXiv](https://img.shields.io/badge/arXiv-1507.08750-b31b1b.svg)](https://arxiv.org/abs/1507.08750)

## World Action Models

- **Faster-WAM**, Faster-WAM: Efficient Inference-Time Future Conditioning for Robust World Action Models. [![arXiv](https://img.shields.io/badge/arXiv-2608.04404-b31b1b.svg)](https://arxiv.org/abs/2608.04404) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/hustvl/FasterWAM)

- **Masked Visual Actions**, Masked Visual Actions for Unified World Modeling. [![arXiv](https://img.shields.io/badge/arXiv-2607.19343-b31b1b.svg)](https://arxiv.org/abs/2607.19343) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://masked-visual-actions.github.io)

- **Temporal Ratio**, Understanding and Mitigating the Video-Action Generalization Gap via Temporal Ratio. [![arXiv](https://img.shields.io/badge/arXiv-2607.08127-b31b1b.svg)](https://arxiv.org/abs/2607.08127) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://umishra.me/temporal-ratio/)

- **LingBot-VA 2**, Native Video-Action Pretraining for Generalizable Robot Control. [![arXiv](https://img.shields.io/badge/arXiv-22607.08639-b31b1b.svg)](https://arxiv.org/abs/2607.08639v1) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://technology.robbyant.com/lingbot-va-v2)

- **FlowWAM**, FlowWAM: Optical Flow as a Unified Action Representation for World Action Models. [![arXiv](https://img.shields.io/badge/arXiv-2607.13017-b31b1b.svg)](https://arxiv.org/abs/2607.13017) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://flow-wam.github.io)

- **WAM-TTT**, WAM-TTT: Steering World-Action Models by Watching Human Play at Test Time. [![arXiv](https://img.shields.io/badge/arXiv-2607.06988-b31b1b.svg)](https://arxiv.org/abs/2607.06988) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://flow-wam.github.io)

- **LaWAM**, LaWAM: Latent World Action Models for Efficient Dynamics-Aware Robot Policies. [![arXiv](https://img.shields.io/badge/arXiv-2606.15768-b31b1b.svg)](https://arxiv.org/html/2606.15768) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://rlinf.github.io/LaWAM/)

- **Next Forcing**, Next Forcing: Causal World Modeling with Multi-Chunk Prediction. [![arXiv](https://img.shields.io/badge/arXiv-2606.11187-b31b1b.svg)](https://arxiv.org/abs/2606.11187) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://gangweix.github.io/next-forcing/)

- **Flash-WAM**, Flash-WAM: Modality-Aware Distillation for World Action Models. [![arXiv](https://img.shields.io/badge/arXiv-2606.05254-b31b1b.svg)](https://arxiv.org/abs/2606.05254) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://flashwam.github.io)

- [⭐️] **Kairos**, Kairos: A Native World Model Stack for Physical AI. [![arXiv](https://img.shields.io/badge/arXiv-2606.1653-b31b1b.svg)](https://arxiv.org/abs/2606.16533) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/kairos-agi/kairos-sensenova)

- **ImageWAM**, ImageWAM: Do World Action Models Really Need Video Generation, or Just Image Editing? [![arXiv](https://img.shields.io/badge/arXiv-2606.19531-b31b1b.svg)](https://arxiv.org/abs/2606.19531) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://zhangwenyao1.github.io/ImageWAM/)

- **GAM**, Geometric Action Model for Robot Policy Learning. [![arXiv](https://img.shields.io/badge/arXiv-2606.17046-b31b1b.svg)](https://arxiv.org/abs/2606.17046) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://cvlab-kaist.github.io/Geometric-Action-Model/)

- [⭐️] **Cosmos 3**, Cosmos 3: Omnimodal World Models for Physical AI. [![arXiv](https://img.shields.io/badge/arXiv-2606.02800-b31b1b.svg)](https://arxiv.org/abs/2606.02800) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://research.nvidia.com/labs/cosmos-lab/cosmos3/)

- **MemoryWAM**, MemoryWAM: Efficient World Action Modeling with Persistent Memory. [![arXiv](https://img.shields.io/badge/arXiv-22606.20562-b31b1b.svg)](https://arxiv.org/abs/2606.20562) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://yangsizhe.github.io/MemoryWAM/)

- **τ0-WM**, τ0-WM: A Unified Video-Action World Model for Robotic Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2606.01027-b31b1b.svg)](https://arxiv.org/abs/2606.01027) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://finch.agibot.com/research/tau0-wm)

- **WAM-RL**, WAM-RL: World-Action Model Reinforcement Learning with Reconstruction Rewards and Online Video SFT. [![arXiv](https://img.shields.io/badge/arXiv-2606.17906-b31b1b.svg)](https://arxiv.org/abs/2606.17906)

- **AdaJEPA**, AdaJEPA: An Adaptive Latent World Model. [![arXiv](https://img.shields.io/badge/arXiv-2606.32026-b31b1b.svg)](https://arxiv.org/abs/2606.32026) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://agenticlearning.ai/adajepa/)

- **GaussianDream**, GaussianDream: A Feed-Forward 3D Gaussian World Model for Robotic Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2605.20752-b31b1b.svg)](https://arxiv.org/abs/2605.20752) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/TuojingAI/GaussianDream)

- **GE-Sim 2.0**, GE-Sim 2.0: A Roadmap Towards Comprehensive Closed-loop Video World Simulators for Robotic Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2605.27491-b31b1b.svg)](https://arxiv.org/abs/2605.27491) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://ge-sim-v2.github.io)

- **Action Images**, Action Images: End-to-End Policy Learning via Multiview Video Generation. [![arXiv](https://img.shields.io/badge/arXiv-2604.06168-b31b1b.svg)](https://arxiv.org/abs/2604.06168) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://actionimages.github.io)

- **DeFI**, Disentangled Robot Learning via Separate Forward and Inverse Dynamics Pretraining. [![arXiv](https://img.shields.io/badge/arXiv-2604.16391-b31b1b.svg)](https://arxiv.org/abs/2604.16391) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/LogosRoboticsGroup/DeFi)

- **Being-H0.7**, Being-H0.7: A Latent World-Action Model from Egocentric Videos. [![arXiv](https://img.shields.io/badge/arXiv-2604-b31b1b.svg)](https://research.beingbeyond.com/projects/being-h07/being-h07.pdf) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://research.beingbeyond.com/being-h07)

- **WAV**, World Action Verifier: Self-Improving World Models via Forward-Inverse Asymmetry. [![arXiv](https://img.shields.io/badge/arXiv-2604.01985-b31b1b.svg)](https://arxiv.org/abs/2604.01985) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://world-action-verifier.github.io)

- **LeWorldModel**, LeWorldModel: Stable End-to-End Joint-Embedding Predictive Architecture from Pixels. [![arXiv](https://img.shields.io/badge/arXiv-2603.19312-b31b1b.svg)](https://arxiv.org/abs/2603.19312) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://le-wm.github.io)

- **GigaWorld-Policy**, GigaWorld-Policy: An Efficient Action-Centered World--Action Model. [![arXiv](https://img.shields.io/badge/arXiv-2603.17240-b31b1b.svg)](https://arxiv.org/abs/2603.17240) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://gigaai-research.github.io/GigaWorld-Policy/)

- [⭐️] **Fast-WAM**, Fast-WAM: Do World Action Models Need Test-time Future Imagination?. [![arXiv](https://img.shields.io/badge/arXiv-2603.16666-b31b1b.svg)](https://arxiv.org/abs/2603.16666) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://yuantianyuan01.github.io/FastWAM/)

- Do World Action Models Generalize Better than VLAs? A Robustness Study. [![arXiv](https://img.shields.io/badge/arXiv-2603.22078-b31b1b.svg)](https://arxiv.org/abs/2603.22078)

- **VLAW**, VLAW: Iterative Co-Improvement of Vision-Language-Action Policy and World Model. [![arXiv](https://img.shields.io/badge/arXiv-2602.12063-b31b1b.svg)](https://arxiv.org/abs/2602.12063) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://sites.google.com/view/vlaw-arxiv)

- [⭐️] **DreamZero**, World Action Models are Zero-shot Policies. [![arXiv](https://img.shields.io/badge/arXiv-2602.15922-b31b1b.svg)](https://arxiv.org/abs/2602.15922) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://dreamzero0.github.io)

- **LDA-1B**, LDA-1B: Scaling Latent Dynamics Action Model via Universal Embodied Data Ingestion. [![arXiv](https://img.shields.io/badge/arXiv-2602.12215-b31b1b.svg)](https://arxiv.org/abs/2602.12215) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://pku-epic.github.io/LDA/)

- **WoG**, World Guidance World Modeling in Condition Space for Action Generation. [![arXiv](https://img.shields.io/badge/arXiv-2602.22010-b31b1b.svg)](https://arxiv.org/abs/2602.22010) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://selen-suyue.github.io/WoGNet/)

- **VLA-JEPA**, VLA-JEPA: Enhancing Vision-Language-Action Model with Latent World Model. [![arXiv](https://img.shields.io/badge/arXiv-2602.10098-b31b1b.svg)](https://arxiv.org/abs/2602.10098) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://ginwind.github.io/VLA-JEPA/)

- [⭐️] **Cosmos Policy**, Cosmos Policy: Fine-Tuning Video Models for Visuomotor Control and Planning. [![arXiv](https://img.shields.io/badge/arXiv-2601.16163-b31b1b.svg)](https://arxiv.org/abs/2601.16163) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://research.nvidia.com/labs/dir/cosmos-policy/)

- [⭐️] **World-VLA-Loop**, World-VLA-Loop: Closed-Loop Learning of Video World Model and VLA Policy. [![arXiv](https://img.shields.io/badge/arXiv-2602.06508-b31b1b.svg)](https://arxiv.org/abs/2602.06508) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://showlab.github.io/World-VLA-Loop/)

- [⭐️] **Lingbot-VA**, Causal World Modeling for Robot Control. [![arXiv](https://img.shields.io/badge/arXiv-2601.21998-b31b1b.svg)](https://arxiv.org/abs/2601.21998) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://technology.robbyant.com/lingbot-va)

- **mimic-video**, mimic-video: Video-Action Models for Generalizable Robot Control Beyond VLAs. [![arXiv](https://img.shields.io/badge/arXiv-2512.15692-b31b1b.svg)](https://arxiv.org/abs/2512.15692) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://mimic-video.github.io)

- **MM-ACT**, MM-ACT: Learn from Multimodal Parallel Generation to Act. [![arXiv](https://img.shields.io/badge/arXiv-2512.00975-b31b1b.svg)](https://arxiv.org/abs/2512.00975) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/HHYHRHY/MM-ACT)

- **RynnVLA-002**, RynnVLA-002: A Unified Vision-Language-Action and World Model. [![arXiv](https://img.shields.io/badge/arXiv-2511.17502-b31b1b.svg)](https://arxiv.org/abs/2511.17502) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/alibaba-damo-academy/RynnVLA-002)

- **WMPO**, WMPO: World Model-based Policy Optimization for Vision-Language-Action Models. [![arXiv](https://img.shields.io/badge/arXiv-2511.09515-b31b1b.svg)](https://arxiv.org/abs/2511.09515)[![Website](https://img.shields.io/badge/Website-Link-blue)](https://wm-po.github.io)

- **World-Env**, World-Env: Leveraging World Model as a Virtual Environment for VLA Post-Training. [![arXiv](https://img.shields.io/badge/arXiv-2509.24948-b31b1b.svg)](https://arxiv.org/abs/2509.24948)[![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/amap-cvlab/world-env)

- **F1**, F1: A Vision-Language-Action Model Bridging Understanding and Generation to Actions. [![arXiv](https://img.shields.io/badge/arXiv-2509.06951-b31b1b.svg)](https://arxiv.org/abs/2509.06951) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://aopolin-lv.github.io/F1-VLA/)

- **FlowVLA**, FlowVLA: Visual Chain of Thought-based Motion Reasoning for Vision-Language-Action Models. [![arXiv](https://img.shields.io/badge/arXiv-2508.18269-b31b1b.svg)](https://arxiv.org/abs/2508.18269) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://irpn-lab.github.io/FlowVLA/)

- **Video Policy**, Video Generators are Robot Policies. [![arXiv](https://img.shields.io/badge/arXiv-2508.00795-b31b1b.svg)](https://arxiv.org/abs/2508.00795) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://videopolicy.cs.columbia.edu)

- **DreamVLA**, DreamVLA: A Vision-Language-Action Model Dreamed with Comprehensive World Knowledge. [![arXiv](https://img.shields.io/badge/arXiv-2507.04447-b31b1b.svg)](https://arxiv.org/abs/2507.04447) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://zhangwenyao1.github.io/DreamVLA/)

- **UniVLA**, Unified Vision-Language-Action Model. [![arXiv](https://img.shields.io/badge/arXiv-2506.19850-b31b1b.svg)](https://arxiv.org/abs/2506.19850) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://robertwyq.github.io/univla.github.io/)

- **WorldVLA**, WorldVLA: Towards Autoregressive Action World Model. [![arXiv](https://img.shields.io/badge/arXiv-2506.21539-b31b1b.svg)](https://arxiv.org/abs/2506.21539) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/alibaba-damo-academy/RynnVLA-002)

- **UniVLA**, UniVLA: Learning to Act Anywhere with Task-centric Latent Actions. [![arXiv](https://img.shields.io/badge/arXiv-2505.06111-b31b1b.svg)](https://arxiv.org/abs/2505.06111) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/OpenDriveLab/UniVLA)

- **DreamGen**, DreamGen: Unlocking Generalization in Robot Learning through Video World Models. [![arXiv](https://img.shields.io/badge/arXiv-2505.12705-b31b1b.svg)](https://arxiv.org/abs/2505.12705) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://research.nvidia.com/labs/gear/dreamgen/)

- **FLARE**, FLARE: Robot Learning with Implicit World Modeling. [![arXiv](https://img.shields.io/badge/arXiv-2505.15659-b31b1b.svg)](https://arxiv.org/abs/2505.15659) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://research.nvidia.com/labs/gear/flare)

- **UWM**, Unified World Models: Coupling Video and Action Diffusion for Pretraining on Large Robotic Datasets. [![arXiv](https://img.shields.io/badge/arXiv-2504.02792-b31b1b.svg)](https://arxiv.org/abs/2504.02792) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://weirdlabuw.github.io/uwm/)

- [⭐️] **UVAM**, Unified Video Action Model. [![arXiv](https://img.shields.io/badge/arXiv-2503.00200-b31b1b.svg)](https://arxiv.org/abs/2503.00200) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://unified-video-action-model.github.io)

- **Inverse Probabilistic Adaptation**, Solving New Tasks by Adapting Internet Video Knowledge. [![arXiv](https://img.shields.io/badge/arXiv-2504.15369-b31b1b.svg)](https://arxiv.org/abs/2504.15369) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://diffusion-supervision.github.io/adapt2act/)

- **CoT-VLA**, CoT-VLA: Visual Chain-of-Thought Reasoning for Vision-Language-Action Models. [![arXiv](https://img.shields.io/badge/arXiv-2503.22020-b31b1b.svg)](https://arxiv.org/abs/2503.22020) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://cot-vla.github.io)

- **UP-VLA**, UP-VLA: A Unified Understanding and Prediction Model for Embodied Agent. [![arXiv](https://img.shields.io/badge/arXiv-2501.18867-b31b1b.svg)](https://arxiv.org/abs/2501.18867) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/CladernyJorn/UP-VLA)

- **VPP**,Video Prediction Policy: A Generalist Robot Policy with Predictive Visual Representations. [![arXiv](https://img.shields.io/badge/arXiv-2412.14803-b31b1b.svg)](https://arxiv.org/abs/2412.14803) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://video-prediction-policy.github.io)

- **NWM**, Navigation World Models. [![arXiv](https://img.shields.io/badge/arXiv-2412.03572-b31b1b.svg)](https://arxiv.org/abs/2412.03572) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://www.amirbar.net/nwm/)

- **Seer**, Predictive Inverse Dynamics Models are Scalable Learners for Robotic Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2412.15109-b31b1b.svg)](https://arxiv.org/abs/2412.15109) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/InternRobotics/Seer)

- **GameGen-X**, GameGen-X: Interactive Open-world Game Video Generation. [![arXiv](https://img.shields.io/badge/arXiv-2411.00769-b31b1b.svg)](https://arxiv.org/abs/2411.00769) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/GameGen-X/GameGen-X)

- **GR-2**, GR-2: A Generative Video-Language-Action Model with Web-Scale Knowledge for Robot Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2410.06158-b31b1b.svg)](https://arxiv.org/abs/2410.06158) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://gr2-manipulation.github.io)

- **GameNGen**, Diffusion Models Are Real-Time Game Engines. [![arXiv](https://img.shields.io/badge/arXiv-2408.14837-b31b1b.svg)](https://arxiv.org/abs/2408.14837) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://gamengen.github.io)

- **DIAMOND**, Diffusion for World Modeling: Visual Details Matter in Atari. [![arXiv](https://img.shields.io/badge/arXiv-2405.12399-b31b1b.svg)](https://arxiv.org/abs/2405.12399) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://diamond-wm.github.io)

- [⭐️] **GR-1**, Unleashing Large-Scale Video Generative Pre-training for Visual Robot Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2312.13139-b31b1b.svg)](https://arxiv.org/abs/2312.13139) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://gr1-manipulation.github.io)

- **VLP**, Video Language Planning. [![arXiv](https://img.shields.io/badge/arXiv-2310.10625-b31b1b.svg)](https://arxiv.org/abs/2310.10625) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://video-language-planning.github.io)

- **UniSim**, Learning Interactive Real-World Simulators. [![arXiv](https://img.shields.io/badge/arXiv-2310.06114-b31b1b.svg)](https://arxiv.org/abs/2310.06114) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://universal-simulator.github.io/unisim/)

- **Dynalang**, Learning to Model the World with Language. [![arXiv](https://img.shields.io/badge/arXiv-2308.01399-b31b1b.svg)](https://arxiv.org/abs/2308.01399) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://dynalang.github.io)

- **UniPi**, Learning Universal Policies via Text-Guided Video Generation. [![arXiv](https://img.shields.io/badge/arXiv-2302.00111-b31b1b.svg)](https://arxiv.org/abs/2302.00111) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://universal-policy.github.io/unipi/)

- [⭐️] **DreamerV3**, Mastering Diverse Domains through World Models. [![arXiv](https://img.shields.io/badge/arXiv-2301.04104-b31b1b.svg)](https://arxiv.org/abs/2301.04104) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://danijar.com/project/dreamerv3/)

- **DayDreamer**, DayDreamer: World Models for Physical Robot Learning. [![arXiv](https://img.shields.io/badge/arXiv-2206.14176-b31b1b.svg)](https://arxiv.org/abs/2206.14176) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://danijar.com/project/daydreamer/)

- **MWM**, Masked World Models for Visual Control. [![arXiv](https://img.shields.io/badge/arXiv-2206.14244-b31b1b.svg)](https://arxiv.org/abs/2206.14244) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://sites.google.com/view/mwm-rl)

- [⭐️] **Diffusers**, Planning with Diffusion for Flexible Behavior Synthesis. [![arXiv](https://img.shields.io/badge/arXiv-2205.09991-b31b1b.svg)](https://arxiv.org/abs/2205.09991) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://diffusion-planning.github.io)

- [⭐️] **DreamerV2**, Mastering Atari with Discrete World Models. [![arXiv](https://img.shields.io/badge/arXiv-2010.02193-b31b1b.svg)](https://arxiv.org/abs/2010.02193) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://danijar.com/project/dreamerv2/)

- [⭐️] **SimPLe**, Model-Based Reinforcement Learning for Atari. [![arXiv](https://img.shields.io/badge/arXiv-1903.00374-b31b1b.svg)](https://arxiv.org/abs/1903.00374) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://sites.google.com/view/modelbasedrlatari/home)

- [⭐️] **Dreamer**, Dream to Control: Learning Behaviors by Latent Imagination. [![arXiv](https://img.shields.io/badge/arXiv-1912.01603-b31b1b.svg)](https://arxiv.org/abs/1912.01603) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/google-research/dreamer)

- [⭐️] **PlaNet**, Learning Latent Dynamics for Planning from Pixels. [![arXiv](https://img.shields.io/badge/arXiv-1811.04551-b31b1b.svg)](https://arxiv.org/abs/1811.04551) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/google-research/planet)

- [⭐️] **World Models**, World Models. [![arXiv](https://img.shields.io/badge/arXiv-1803.10122-b31b1b.svg)](https://arxiv.org/abs/1803.10122) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://worldmodels.github.io)

- [⭐️] **Dyna**, Integrated Architectures for Learning, Planning, and Reacting Based on Approximating Dynamic Programming. [![Paper](https://img.shields.io/badge/Paper-Link-blue)](https://www.sciencedirect.com/science/chapter/edited-volume/abs/pii/B9781558601413500304)


## Policies

- **ActionMap**, ActionMap: Robot Policy Learning via Voxel Action Heatmap. [![arXiv](https://img.shields.io/badge/arXiv-2606.06904-b31b1b.svg)](https://arxiv.org/abs/2606.06904) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://showlab.github.io/ActionMap/)

- **Know Your Camera**, Do You Know Where Your Camera Is? View-Invariant Policy Learning with Camera Conditioning. [![arXiv](https://img.shields.io/badge/arXiv-2510.02268-b31b1b.svg)](https://arxiv.org/abs/2510.02268) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://ripl.github.io/know_your_camera/)

- **State-free Policy**, Do You Need Proprioceptive States in Visuomotor Policies?. [![arXiv](https://img.shields.io/badge/arXiv-2509.18644-b31b1b.svg)](https://arxiv.org/abs/2509.18644) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://statefreepolicy.github.io)

- **LBM**, A Careful Examination of Large Behavior Models for Multitask Dexterous Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2507.05331-b31b1b.svg)](https://arxiv.org/abs/2507.05331) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://toyotaresearchinstitute.github.io/lbm1/)

- **Adapt Your Body**, Adapt Your Body: Mitigating Proprioception Shifts in Imitation Learning. [![arXiv](https://img.shields.io/badge/arXiv-2506.23944-b31b1b.svg)](https://arxiv.org/abs/2506.23944v1)

- **RDP**, Reactive Diffusion Policy: Slow-Fast Visual-Tactile Policy Learning for Contact-Rich Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2503.02881-b31b1b.svg)](https://arxiv.org/abs/2503.02881) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://reactive-diffusion-policy.github.io)

- [⭐️] Data Scaling Laws in Imitation Learning for Robotic Manipulationy. [![arXiv](https://img.shields.io/badge/arXiv-2410.18647-b31b1b.svg)](https://arxiv.org/abs/2410.18647)

- [⭐️] **RDT-1B**, RDT-1B: a Diffusion Foundation Model for Bimanual Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2410.07864-b31b1b.svg)](https://arxiv.org/abs/2410.07864) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://rdt-robotics.github.io/rdt-robotics/)

- **HPT**, Scaling Proprioceptive-Visual Learning with Heterogeneous Pre-trained Transformers. [![arXiv](https://img.shields.io/badge/arXiv-2409.20537-b31b1b.svg)](https://arxiv.org/abs/2409.20537) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://liruiw.github.io/hpt/)

- **MDT**, Multimodal Diffusion Transformer: Learning Versatile Behavior from Multimodal Goals. [![arXiv](https://img.shields.io/badge/arXiv-2407.05996-b31b1b.svg)](https://arxiv.org/abs/2407.05996) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://intuitive-robots.github.io/mdt_policy/)

- [⭐️] **Octo**, Octo: An Open-Source Generalist Robot Policy. [![arXiv](https://img.shields.io/badge/arXiv-2405.12213-b31b1b.svg)](https://arxiv.org/abs/2405.12213) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://octo-models.github.io)

- **ManiGaussian**, ManiGaussian: Dynamic Gaussian Splatting for Multi-task Robotic Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2403.08321-b31b1b.svg)](https://arxiv.org/abs/2403.08321) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://guanxinglu.github.io/ManiGaussian/)

- [⭐️] **DP3**, 3D Diffusion Policy: Generalizable Visuomotor Policy Learning via Simple 3D Representations. [![arXiv](https://img.shields.io/badge/arXiv-2403.03954-b31b1b.svg)](https://arxiv.org/abs/2403.03954) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://3d-diffusion-policy.github.io)

- **RPT**, Robot Learning with Sensorimotor Pre-training. [![arXiv](https://img.shields.io/badge/arXiv-2306.10007-b31b1b.svg)](https://arxiv.org/abs/2306.10007) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://robotic-pretrained-transformer.github.io)

- [⭐️] **Diffusion Policy**, Diffusion Policy: Visuomotor Policy Learning via Action Diffusion. [![arXiv](https://img.shields.io/badge/arXiv-2303.04137-b31b1b.svg)](https://arxiv.org/abs/2303.04137) [![Website](https://img.shields.io/badge/Website-Link-blue)](http://diffusion-policy.cs.columbia.edu)

- [⭐️] **RT-1**, RT-1: Robotics Transformer for Real-World Control at Scale. [![arXiv](https://img.shields.io/badge/arXiv-2212.06817-b31b1b.svg)](https://arxiv.org/abs/2212.06817) [![Website](https://img.shields.io/badge/Website-Link-blue)](http://robotics-transformer1.github.io)

- [⭐️] **PerAct**, Perceiver-Actor: A Multi-Task Transformer for Robotic Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2209.05451-b31b1b.svg)](https://arxiv.org/abs/2209.05451) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://peract.github.io)

## Latent Action Models

- **LAWM-3D**, LAWM-3D: Learning 3D-Aware Latent Actions from Human Videos for Generalizable Robot World Models. [![arXiv](https://img.shields.io/badge/arXiv-2608.05706-b31b1b.svg)](https://arxiv.org/abs/2608.05706)

- [⭐️] **LARA**, LARA: Latent Action Representation Alignment for Vision-Language-Action Models. [![arXiv](https://img.shields.io/badge/arXiv-2606.07100-b31b1b.svg)](https://arxiv.org/abs/2606.07100) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://lmy1001.github.io/ICML26_LARA/)

- **DiLA**, DiLA: Disentangled Latent Action World Models. [![arXiv](https://img.shields.io/badge/arXiv-2605.15725-b31b1b.svg)](https://arxiv.org/abs/2605.15725) [![Website](https://img.shields.io/badge/Website-Link-blue)](http://disentangled-latent-action-world-models.github.io)

- **From Pixels to Tokens**, From Pixels to Tokens: A Systematic Study of Latent Action Supervision for Vision-Language-Action Models. [![arXiv](https://img.shields.io/badge/arXiv-2605.04678-b31b1b.svg)](https://arxiv.org/abs/2605.04678) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/RUCKBReasoning/From_Pixels_to_Tokens)

- **HiLAM**, Hierarchical Latent Action Model. [![arXiv](https://img.shields.io/badge/arXiv-2603.05815-b31b1b.svg)](https://arxiv.org/abs/2603.05815)

- [⭐️] **DreamDojo**, DreamDojo: A Generalist Robot World Model from Large-Scale Human Videos. [![arXiv](https://img.shields.io/badge/arXiv-2602.06949-b31b1b.svg)](https://arxiv.org/abs/2602.06949) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://dreamdojo-world.github.io)

- [⭐️] Learning Latent Action World Models In The Wild. [![arXiv](https://img.shields.io/badge/arXiv-2601.05230-b31b1b.svg)](https://arxiv.org/pdf/2601.05230)

- **Motus**, Motus: A Unified Latent Action World Model. [![arXiv](https://img.shields.io/badge/arXiv-2512.13030-b31b1b.svg)](https://arxiv.org/abs/2512.13030) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://motus-robotics.github.io/motus)

- **CoLA-World**, Co-Evolving Latent Action World Models. [![arXiv](https://img.shields.io/badge/arXiv-2510.26433-b31b1b.svg)](https://arxiv.org/abs/2510.26433)

- **LPS**, Latent Policy Steering with Embodiment-Agnostic Pretrained World Models. [![arXiv](https://img.shields.io/badge/arXiv-2507.13340-b31b1b.svg)](https://arxiv.org/abs/2507.13340)

- **CoMo**, CoMo: Learning Continuous Latent Motion from Internet Videos for Scalable Robot Learning. [![arXiv](https://img.shields.io/badge/arXiv-2505.17006-b31b1b.svg)](https://arxiv.org/abs/2505.17006) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/MCG-NJU/CoMo)

- [⭐️] **GR00T N1**, GR00T N1: An Open Foundation Model for Generalist Humanoid Robots. [![arXiv](https://img.shields.io/badge/arXiv-2503.14734-b31b1b.svg)](https://arxiv.org/abs/2503.14734) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://developer.nvidia.com/isaac/gr00t)

- **AdaWorld**, AdaWorld: Learning Adaptable World Models with Latent Actions. [![arXiv](https://img.shields.io/badge/arXiv-2503.18938-b31b1b.svg)](https://arxiv.org/abs/2503.18938) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://adaptable-world-model.github.io)

- **Moto**, Moto: Latent Motion Token as the Bridging Language for Learning Robot Manipulation from Videos. [![arXiv](https://img.shields.io/badge/arXiv-2412.04445-b31b1b.svg)](https://arxiv.org/abs/2412.04445) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://chenyi99.github.io/moto/)

- [⭐️] **LAPA**, Latent Action Pretraining from Videos. [![arXiv](https://img.shields.io/badge/arXiv-2410.11758-b31b1b.svg)](https://arxiv.org/abs/2410.11758) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://latentactionpretraining.github.io)

- [⭐️] **Genie**, Genie: Generative Interactive Environments. [![arXiv](https://img.shields.io/badge/arXiv-2402.15391-b31b1b.svg)](https://arxiv.org/abs/2402.15391) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://sites.google.com/view/genie-2024/)

- **LAPO**, Learning to Act without Actions. [![arXiv](https://img.shields.io/badge/arXiv-2312.10812-b31b1b.svg)](https://arxiv.org/abs/2312.10812) [![Website](https://img.shields.io/badge/Website-Link-blue)](http://github.com/schmidtdominik/LAPO)

- **AVDC**, Learning to Act from Actionless Videos through Dense Correspondences. [![arXiv](https://img.shields.io/badge/arXiv-2310.08576-b31b1b.svg)](https://arxiv.org/abs/2310.08576) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://flow-diffusion.github.io)

- **CLASP**, Learning what you can do before doing anything. [![arXiv](https://img.shields.io/badge/arXiv-1806.09655-b31b1b.svg)](https://arxiv.org/abs/1806.09655)[![Website](https://img.shields.io/badge/Website-Link-blue)](https://daniilidis-group.github.io/learned_action_spaces/)

- **ILPO**, Imitating Latent Policies from Observation. [![arXiv](https://img.shields.io/badge/arXiv-1805.07914-b31b1b.svg)](https://arxiv.org/abs/1805.07914) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/ashedwards/ILPO)

## Human Action Pretraining

- [⭐️] **Xiaomi-Robotics-1**, Xiaomi-Robotics-1: Scaling Vision-Language-Action Models with over 100K Hours of Real-World Trajectories. [![arXiv](https://img.shields.io/badge/arXiv-2607.15330-b31b1b.svg)](https://arxiv.org/abs/2607.15330) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://robotics.xiaomi.com/xiaomi-robotics-1.html)

- [⭐️] **HumanScale**, HumanScale: Egocentric Human Video Can Outperform Real-Robot Data for Embodied Pretraining. [![arXiv](https://img.shields.io/badge/arXiv-2606.20521-b31b1b.svg)](https://arxiv.org/abs/2606.20521) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/DAGroup-PKU/HumanNet/)

- **HumanEgo**, HumanEgo: Zero-Shot Robot Learning from Minutes of Human Egocentric Videos. [![arXiv](https://img.shields.io/badge/arXiv-2605.24934-b31b1b.svg)](https://arxiv.org/abs/2605.24934) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://humanego-ai.github.io)

- **Being-H0.7**, Being-H0.7: A Latent World-Action Model from Egocentric Videos. [![arXiv](https://img.shields.io/badge/arXiv-2604-b31b1b.svg)](https://research.beingbeyond.com/projects/being-h07/being-h07.pdf) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://research.beingbeyond.com/being-h07)

- [⭐️] **Egoscale**, EgoScale: Scaling Dexterous Manipulation with Diverse Egocentric Human Data. [![arXiv](https://img.shields.io/badge/arXiv-2602.16710-b31b1b.svg)](https://arxiv.org/abs/2602.16710) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://research.nvidia.com/labs/gear/egoscale/)

- [⭐️] Emergence of Human to Robot Transfer in Vision-Language-Action Models. [![arXiv](https://img.shields.io/badge/arXiv-2512.22414-b31b1b.svg)](https://arxiv.org/abs/2512.22414) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://www.pi.website/research/human_to_robot)

- [⭐️] **EgoVLA**, EgoVLA: Learning Vision-Language-Action Models from Egocentric Human Videos. [![arXiv](https://img.shields.io/badge/arXiv-2507.12440-b31b1b.svg)](https://arxiv.org/abs/2507.12440) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://rchalyang.github.io/EgoVLA/)

## Code as Policy

- **OpenETA**, ETA: A New Agentic Paradigm for Embodied Tasks. [![arXiv](https://img.shields.io/badge/arXiv-2608.03924-b31b1b.svg)](https://arxiv.org/abs/2608.03924) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://openmoss.ai/OpenETA/)

- [⭐️] **Gemini Robotics 2**, Gemini Robotics 2: The intelligence layer to power any kind of robot. [![Website](https://img.shields.io/badge/Website-Link-blue)](https://deepmind.google/models/gemini-robotics/)

- **Harness VLA**, Harness VLA: Steering Frozen VLAs into Reliable Manipulation Primitives via Memory-Guided Agents. [![arXiv](https://img.shields.io/badge/arXiv-2607.08448-b31b1b.svg)](https://arxiv.org/abs/2607.08448) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://harnessvla.github.io)

- **CaP-X**, CaP-X: A Framework for Benchmarking and Improving Coding Agents for Robot Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2603.22435-b31b1b.svg)](https://arxiv.org/abs/2603.22435) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://capgym.github.io)

- **Dream2Flow**, Dream2Flow: Bridging Video Generation and Open-World Manipulation with 3D Object Flow. [![arXiv](https://img.shields.io/badge/arXiv-2512.24766-b31b1b.svg)](https://arxiv.org/abs/2512.24766) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://dream2flow.github.io)

- **ReKep**, ReKep: Spatio-Temporal Reasoning of Relational Keypoint Constraints for Robotic Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2409.01652-b31b1b.svg)](https://arxiv.org/abs/2409.01652) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://rekep-robot.github.io)

- **VoxPoser**, VoxPoser: Composable 3D Value Maps for Robotic Manipulation with Language Models. [![arXiv](https://img.shields.io/badge/arXiv-2307.05973-b31b1b.svg)](https://arxiv.org/abs/2307.05973) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://voxposer.github.io)

- [⭐️] **Code as Policies**, Code as Policies: Language Model Programs for Embodied Control. [![arXiv](https://img.shields.io/badge/arXiv-2209.07753-b31b1b.svg)](https://arxiv.org/abs/2209.07753) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://code-as-policies.github.io)

- [⭐️] **Zero-Shot Planner**, Language Models as Zero-Shot Planners: Extracting Actionable Knowledge for Embodied Agents. [![arXiv](https://img.shields.io/badge/arXiv-2201.07207-b31b1b.svg)](https://arxiv.org/abs/2201.07207) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://wenlonghuang.com/language-planner/)

## Survey

- Data Pyramid for Embodied Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2607.24744-b31b1b.svg)](https://arxiv.org/abs/2607.24744) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://jasper-aaa.github.io/embodied-data-pyramid/)

- Safety in Embodied AI: A Survey of Risks, Attacks, and Defenses. [![arXiv](https://img.shields.io/badge/arXiv-2605.02900-b31b1b.svg)](https://arxiv.org/abs/2605.02900) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://x-zheng16.github.io/Awesome-Embodied-AI-Safety/)

- Vision-Language-Action (VLA) Models: Concepts, Progress, Applications and Challenges. [![arXiv](https://img.shields.io/badge/arXiv-2505.04769-b31b1b.svg)](https://arxiv.org/abs/2505.04769) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/Applied-AI-Research-Lab/Vision-Language-Action-Models-Concepts-Progress-Applications-and-Challenges)

- Vision-Language-Action Safety: Threats, Challenges, Evaluations, and Mechanisms. [![arXiv](https://img.shields.io/badge/arXiv-2604.23775-b31b1b.svg)](https://arxiv.org/abs/2604.23775) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/LiQiiiii/Awesome-VLA-Safety)

- A Survey on Vision-Language-Action Models for Embodied AI. [![arXiv](https://img.shields.io/badge/arXiv-2405.14093-b31b1b.svg)](https://arxiv.org/abs/2405.14093) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/yueen-ma/Awesome-VLA)

## Robotics Datasets

- [⭐️] **ABC-130k**, Scalable Behavior Cloning with Open Data, Training, and Evaluation. [![arXiv](https://img.shields.io/badge/arXiv-2606.27375-b31b1b.svg)](https://arxiv.org/abs/2606.27375) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://abc.bot)

- **GM100**, The Great March 100: 100 Detail-oriented Tasks for Evaluating Embodied AI Agents. [![arXiv](https://img.shields.io/badge/arXiv-2601.11421-b31b1b.svg)](https://arxiv.org/abs/2601.11421) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://www.rhos.ai/research/gm-100)

- **RoboMIND 2.0**, RoboMIND 2.0: A Multimodal, Bimanual Mobile Manipulation Dataset for Generalizable Embodied Intelligence. [![arXiv](https://img.shields.io/badge/arXiv-2512.24653-b31b1b.svg)](https://arxiv.org/abs/2512.24653) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://www.modelscope.cn/collections/X-Humanoid/RoboMIND20)

- **RoboCOIN**, RoboCOIN: An Open-Sourced Bimanual Robotic Data COllection for INtegrated Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2511.17441-b31b1b.svg)](https://arxiv.org/abs/2511.17441) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://flagopen.github.io/RoboCOIN/)

- **Humanoid Everyday**, Humanoid Everyday: A Comprehensive Robotic Dataset for Open-World Humanoid Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2510.08807-b31b1b.svg)](https://arxiv.org/abs/2510.08807) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://humanoideveryday.github.io)

- **Fourier ActionNet Dataset**, Fourier ActionNet Dataset. [![Website](https://img.shields.io/badge/Website-Link-blue)](https://action-net.org)

- **Galaxea**, Galaxea Open-World Dataset and G0 Dual-System VLA Model. [![arXiv](https://img.shields.io/badge/arXiv-2509.00576-b31b1b.svg)](https://arxiv.org/abs/2509.00576) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://huggingface.co/datasets/OpenGalaxea/Galaxea-Open-World-Dataset)

- **MolmoAct**, MolmoAct: Action Reasoning Models that can Reason in Space. [![arXiv](https://img.shields.io/badge/arXiv-2508.07917-b31b1b.svg)](https://arxiv.org/abs/2508.07917) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://allenai.org/blog/molmoact)

- [⭐️] **AgiBot World**, AgiBot World Colosseo: A Large-scale Manipulation Platform for Scalable and Intelligent Embodied Systems. [![arXiv](https://img.shields.io/badge/arXiv-2503.06669-b31b1b.svg)](https://arxiv.org/abs/2503.06669) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://agibot-world.com)

- **RoboMIND**, RoboMIND: Benchmark on Multi-embodiment Intelligence Normative Data for Robot Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2412.13877-b31b1b.svg)](https://arxiv.org/abs/2412.13877) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://x-humanoid-robomind.github.io)

- [⭐️] **DROID**, DROID: A Large-Scale In-The-Wild Robot Manipulation Dataset. [![arXiv](https://img.shields.io/badge/arXiv-2403.12945-b31b1b.svg)](https://arxiv.org/abs/2403.12945) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://droid-dataset.github.io)

- [⭐️] **Open X-Embodiment**, Open X-Embodiment: Robotic Learning Datasets and RT-X Models. [![arXiv](https://img.shields.io/badge/arXiv-2310.08864-b31b1b.svg)](https://arxiv.org/abs/2310.08864) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://robotics-transformer-x.github.io)

- **RH20T**, RH20T: A Comprehensive Robotic Dataset for Learning Diverse Skills in One-Shot. [![arXiv](https://img.shields.io/badge/arXiv-2307.00595-b31b1b.svg)](https://arxiv.org/abs/2307.00595) [![Website](https://img.shields.io/badge/Website-Link-blue)](http://rh20t.github.io)


## Ego Human Datasets

- [⭐️] **Open-AoE**, Open-AoE: An Open Egocentric Manipulation Dataset and Toolchain for Embodied Learning. [![arXiv](https://img.shields.io/badge/arXiv-2607.14183-b31b1b.svg)](https://arxiv.org/abs/2607.14183) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/ant-research/Open-AoE)

- **HiFi-UMI**, HiFi-UMI: Learning Deployable Manipulation Policies from High-Fidelity UMI Data Alone. [![arXiv](https://img.shields.io/badge/arXiv-2607.25895-b31b1b.svg)](https://arxiv.org/abs/2607.25895) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://cloud.simpleai.tech/simple-world-lab/hifi-umi/)

- **ActiveMimic**, ActiveMimic: Egocentric Video Pretraining with Active Perception. [![arXiv](https://img.shields.io/badge/arXiv-2606.06194-b31b1b.svg)](https://arxiv.org/abs/2606.06194) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://activemimic.github.io)

- **HumanNet**, HumanNet: Scaling Human-centric Video Learning to One Million Hours. [![arXiv](https://img.shields.io/badge/arXiv-2605.06747-b31b1b.svg)](https://arxiv.org/abs/2605.06747) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://dagroup-pku.github.io/HumanNet)

- **EgoVerse**, EgoVerse: An Egocentric Human Dataset for Robot Learning from Around the World. [![arXiv](https://img.shields.io/badge/arXiv-2604.07607-b31b1b.svg)](https://arxiv.org/abs/2604.07607) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://egoverse.ai)

- **xperience-10m**, Xperience-10M: The Largest Human Xperience Dataset. [![Website](https://img.shields.io/badge/Website-Link-blue)](https://ropedia.com/blog/20260316_xperience_10m)

- [⭐️] **EgoDex**, EgoDex: Learning Dexterous Manipulation from Large-Scale Egocentric Video. [![arXiv](https://img.shields.io/badge/arXiv-2505.11709-b31b1b.svg)](https://arxiv.org/abs/2505.11709) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/apple/ml-egodex)

- [⭐️] **Ego4D**, Ego4D: Around the World in 3,000 Hours of Egocentric Video. [![arXiv](https://img.shields.io/badge/arXiv-2110.07058-b31b1b.svg)](https://arxiv.org/pdf/2110.07058) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://ego4d-data.org)

- [⭐️] **Something-Something v2**, The "something something" video database for learning and evaluating visual common sense. [![arXiv](https://img.shields.io/badge/arXiv-1706.04261-b31b1b.svg)](https://arxiv.org/abs/1706.04261) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://www.qualcomm.com/developer/software/something-something-v-2-dataset)


## Benchmark / Environment

- **RoboDojo**, RoboDojo: A Unified Sim-and-Real Benchmark for Comprehensive Evaluation of Generalist Robot Manipulation Policies. [![arXiv](https://img.shields.io/badge/arXiv-2607.04434-b31b1b.svg)](https://arxiv.org/abs/2607.04434) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://robodojo-benchmark.com)

- [⭐️] **RoboLab**, RoboLab: A High-Fidelity Simulation Benchmark for Analysis of Task Generalist Policies. [![arXiv](https://img.shields.io/badge/arXiv-2604.09860-b31b1b.svg)](https://arxiv.org/abs/2604.09860) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://research.nvidia.com/labs/srl/projects/robolab/)

- [⭐️] **WorldArena**, WorldArena: A Unified Benchmark for Evaluating Perception and Functional Utility of Embodied World Models. [![arXiv](https://img.shields.io/badge/arXiv-2602.08971-b31b1b.svg)](https://arxiv.org/abs/2602.08971) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://world-arena.ai)

- **PAI-Bench**, PAI-Bench: A Comprehensive Benchmark For Physical AI. [![arXiv](https://img.shields.io/badge/arXiv-2512.01989-b31b1b.svg)](https://arxiv.org/abs/2512.01989) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/SHI-Labs/physical-ai-bench)

- **LIBERO-Plus**, LIBERO-Plus: In-depth Robustness Analysis of Vision-Language-Action Models. [![arXiv](https://img.shields.io/badge/arXiv-2510.13626-b31b1b.svg)](https://arxiv.org/abs/2510.13626) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://sylvestf.github.io/LIBERO-plus/)

- **RoboChallenge**, RoboChallenge: Large-scale Real-robot Evaluation of Embodied Policies. [![arXiv](https://img.shields.io/badge/arXiv-2510.17950-b31b1b.svg)](https://arxiv.org/abs/2510.17950) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://robochallenge.ai/home)

- [⭐️] **RoboArena**, RoboArena: Distributed Real-World Evaluation of Generalist Robot Policies. [![arXiv](https://img.shields.io/badge/arXiv-2506.18123-b31b1b.svg)](https://arxiv.org/abs/2506.18123) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://robo-arena.github.io)

- [⭐️] **RoboTwin 2.0**, RoboTwin 2.0: A Scalable Data Generator and Benchmark with Strong Domain Randomization for Robust Bimanual Robotic Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2506.18088-b31b1b.svg)](https://arxiv.org/abs/2506.18088) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/robotwin-Platform/robotwin/)

- [⭐️] **RoboCasa**, RoboCasa: Large-Scale Simulation of Everyday Tasks for Generalist Robots. [![arXiv](https://img.shields.io/badge/arXiv-2406.02523-b31b1b.svg)](https://arxiv.org/abs/2406.02523) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://robocasa.ai)

- [⭐️] **SimplerEnv**, Evaluating Real-World Robot Manipulation Policies in Simulation. [![arXiv](https://img.shields.io/badge/arXiv-2405.05941-b31b1b.svg)](https://arxiv.org/abs/2405.05941) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://simpler-env.github.io)

- [⭐️] **LIBERO**, LIBERO: Benchmarking Knowledge Transfer for Lifelong Robot Learning. [![arXiv](https://img.shields.io/badge/arXiv-2306.03310-b31b1b.svg)](https://arxiv.org/abs/2306.03310) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://libero-project.github.io/main.html)

- **FurnitureBench**, FurnitureBench: Reproducible Real-World Benchmark for Long-Horizon Complex Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2305.12821-b31b1b.svg)](https://arxiv.org/abs/2305.12821) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://clvrai.github.io/furniture-bench/)

- [⭐️] **CALVIN**, CALVIN: A Benchmark for Language-Conditioned Policy Learning for Long-Horizon Robot Manipulation Tasks. [![arXiv](https://img.shields.io/badge/arXiv-2112.03227-b31b1b.svg)](https://arxiv.org/abs/2112.03227) [![Website](https://img.shields.io/badge/Website-Link-blue)](http://calvin.cs.uni-freiburg.de)

- [⭐️] **SAPIEN**, SAPIEN: A SimulAted Part-based Interactive ENvironment. [![arXiv](https://img.shields.io/badge/arXiv-2003.08515-b31b1b.svg)](https://arxiv.org/abs/2003.08515) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://sapien.ucsd.edu)

- [⭐️] **RLBench**, RLBench: The Robot Learning Benchmark & Learning Environment. [![arXiv](https://img.shields.io/badge/arXiv-1909.12271-b31b1b.svg)](https://arxiv.org/abs/1909.12271) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://sites.google.com/view/rlbench)

## Physics Engine

- [⭐️] **PhysX**, [![Website](https://img.shields.io/badge/Website-Link-blue)](https://developer.nvidia.com/physx-sdk)

- [⭐️] **MuJoCo**. [![Website](https://img.shields.io/badge/Website-Link-blue)](https://mujoco.org)

- [⭐️] **PyBullet**. [![Website](https://img.shields.io/badge/Website-Link-blue)](https://pybullet.org/wordpress/)

## Software

- **Embodied.cpp**, Embodied.cpp: A Portable Inference Runtime of Embodied AI Models on Heterogeneous Robots. [![arXiv](https://img.shields.io/badge/arXiv-2607.02501-b31b1b.svg)](https://arxiv.org/abs/2607.02501) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://github.com/SEU-PAISys/Embodied.cpp)

- [⭐️] **ROS**, Robot Operating System. [![arXiv](https://img.shields.io/badge/arXiv-2009-b31b1b.svg)](https://ai.stanford.edu/~mquigley/papers/icra2009-ros.pdf) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://www.ros.org)

## Hardware

- **HiFi-UMI**, HiFi-UMI: Learning Deployable Manipulation Policies from High-Fidelity UMI Data Alone. [![arXiv](https://img.shields.io/badge/arXiv-2607.25895-b31b1b.svg)](https://arxiv.org/abs/2607.25895) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://cloud.simpleai.tech/simple-world-lab/hifi-umi/)

- **DexUMI**, DexUMI: Using Human Hand as the Universal Manipulation Interface for Dexterous Manipulation. [![arXiv](https://img.shields.io/badge/arXiv-2505.21864-b31b1b.svg)](https://arxiv.org/abs/2505.21864) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://dex-umi.github.io)

- [⭐️] **UMI**, Universal Manipulation Interface: In-The-Wild Robot Teaching Without In-The-Wild Robots. [![arXiv](https://img.shields.io/badge/arXiv-2402.10329-b31b1b.svg)](https://arxiv.org/abs/2402.10329) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://umi-gripper.github.io)

- **GELLO**, GELLO: A General, Low-Cost, and Intuitive Teleoperation Framework for Robot Manipulators. [![arXiv](https://img.shields.io/badge/arXiv-2309.13037-b31b1b.svg)](https://arxiv.org/abs/2309.13037) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://wuphilipp.github.io/gello_site/)

- [⭐️] **ALOHA**, Learning Fine-Grained Bimanual Manipulation with Low-Cost Hardware. [![arXiv](https://img.shields.io/badge/arXiv-2304.13705-b31b1b.svg)](https://arxiv.org/abs/2304.13705) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://tonyzhaozh.github.io/aloha/)

## Acknowledgements
Thanks to [Awesome World Models](https://github.com/knightnemo/Awesome-World-Models/tree/main) for the template.
