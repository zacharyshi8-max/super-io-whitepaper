# Super IO Interface — Whitepaper References

> Compilation Date: 2026-05-30
> Search Scope: GitHub Open-Source Projects + ArXiv Academic Papers
> Topics: LLM-Driven Multi-Device Collaboration, IoT Data Fusion, Semantic Interoperability

---

## I. Most Directly Relevant Projects (LLM + Multi-Robot / Multi-Device Collaboration)

| Project | Description | Link |
|------|------|------|
| **RoCo: Dialectic Multi-Robot Collaboration with LLMs** | Proposes using pretrained LLMs to simultaneously handle high-level multi-robot communication and low-level path planning. Robots negotiate task strategies and generate motion plans through LLM dialogue. Includes RoCoBench, a 6-task benchmark suite. **Highly aligned with Super IO's core concept of "devices collaborating through LLM dialogue."** | https://github.com/vignesh-anand/robot-collab-v2 |
| **MeCo: LLM-Empowered Multi-Robot via Similar Task Memoization** | A "cache-reuse" framework for multi-robot collaboration that avoids redundant LLM planning calls by matching similar tasks. Latest from 2026. | https://arxiv.org/pdf/2601.20577 |
| **CoCoL: Communication Efficient Decentralized Collaborative Learning** | An efficient communication method for heterogeneous multi-robot systems, addressing data heterogeneity and communication bandwidth challenges. | https://arxiv.org/pdf/2508.20898 |
| **Retrospective Actor-Critic Framework for Multi-Robot** | Introduces the Actor-Critic architecture from reinforcement learning into multi-robot LLM collaboration, where actors make real-time decisions and critics perform retrospective evaluation. | https://arxiv.org/pdf/2502.11227 |

## II. Collaborative Perception / Multi-Device Fusion (V2X / Collaborative Perception)

These projects originate from the autonomous driving V2X domain, but **the technical architecture of inter-device collaborative perception can be directly adapted to Super IO's heterogeneous device data fusion**:

| Project | Description | Link |
|------|------|------|
| **coperception/STAR (CoRL 2022)** | Multi-robot scene completion and collaborative perception framework, including collaborative perception algorithms under V2V/V2X communication modes | https://github.com/coperception/star |
| **ai4ce/DiscoNet (NeurIPS 2021)** | Knowledge-distillation-driven multi-agent collaborative perception graph network, solving information sharing under multi-device communication bandwidth constraints | https://github.com/ai4ce/DiscoNet |
| **MediaBrain-SJTU/SyncNet (ECCV 2022)** | Latency-aware collaborative perception framework, addressing perception fusion problems caused by unsynchronized device clocks in real-world scenarios | https://github.com/MediaBrain-SJTU/SyncNet |
| **CollaborativePerception/V2Xverse** | Comprehensive V2X collaborative perception simulation and benchmark platform, covering collaborative driving scenarios | https://github.com/CollaborativePerception/V2Xverse |
| **Xuezhenggdut/Collaborative_Perception** | A curated collection of papers in the collaborative/cooperative/multi-agent perception domain, containing 90+ paper summaries | https://github.com/Xuezhenggdut/Collaborative_Perception |
| **dempsey-wen/SiMO** | A unimodal-operable multimodal collaborative perception solution | https://github.com/dempsey-wen/SiMO |

## III. VLM / Vision-Language Models + Robot Navigation

| Project | Description | Link |
|------|------|------|
| **SimoneMic/vlmaps (ICRA 2023)** | Visual Language Maps — fuses pretrained VLM features into 3D spatial reconstruction, enabling robots to navigate and retrieve information in environments using natural language. **Directly related to Super IO's "cameras understanding scenes + robots executing tasks" paradigm.** | https://github.com/SimoneMic/vlmaps |
| **marooncn/navbot** | Map-less robot navigation using RGB images as visual input, featuring three-tier navigation capabilities: memory, reasoning, and exploration | https://github.com/marooncn/navbot |

## IV. IoT Platforms + Large Model Integration

| Project | Description | Link |
|------|------|------|
| **acon96/home-llm** (687 commits) | Home Assistant integration that uses a **fully localized LLM** to control smart home devices. No cloud services required, privacy-first. **Closest to Super IO's vision of "LLM-based unified control of heterogeneous IoT devices."** | https://github.com/acon96/home-llm |
| **ITSpecialist111/ai_automation_suggester** (208 commits) | AI-driven Home Assistant automation suggestion engine. The LLM scans all device entities and intelligently recommends YAML automation rules. **Demonstrates the capability of "LLM understanding all device semantics and generating cross-device automation strategies."** | https://github.com/ITSpecialist111/ai_automation_suggester |
| **thingsboard/thingsboard** | Open-source IoT platform — device management, data collection, processing, and visualization, including a rule engine and MQTT transport layer | https://github.com/thingsboard/thingsboard |
| **thin-edge.io** | Lightweight IoT edge framework with sub-device registration and management plugins | https://github.com/thin-edge/device-registration-server |

## V. Edge AI and On-Device LLM

These technologies are key infrastructure for realizing "on-device agents + Super IO edge preprocessing":

| Project | Description | Link |
|------|------|------|
| **MLC LLM (mlc-ai/mlc-llm)** | Universal LLM deployment framework — any language model can be natively deployed to diverse hardware backends (mobile / edge / browser) | https://github.com/mlc-ai/mlc-llm |
| **Microsoft Semantic Kernel** | Enterprise-grade AI Agent orchestration framework, model-agnostic SDK supporting the construction and deployment of multi-agent systems. **Can serve as Super IO's agent orchestration layer.** | https://github.com/microsoft/semantic-kernel |
| **LF Edge** | Linux Foundation edge computing organization, defining open and interoperable edge framework standards | https://github.com/lf-edge |

## VI. Communication / Protocol Layer Infrastructure

| Project | Description | Link |
|------|------|------|
| **Eclipse Hono / Eclipse SDV Fleet Management** | Eclipse Foundation connected-vehicle device management blueprint, featuring MQTT-based device registration, telemetry, and command dispatch | https://github.com/eclipse-sdv-blueprints/fleet-management |
| **ntex-rs/ntex-mqtt** | High-performance MQTT v5/v3.1.1 protocol framework implemented in Rust | https://github.com/ntex-rs/ntex-mqtt |

## VII. Key Academic Paper Checklist

| Paper | Venue | Core Contribution |
|------|------|----------|
| RoCo: Dialectic Multi-Robot Collaboration with LLMs | arXiv 2307.04738 | LLM as a conversational collaboration engine for multi-robot systems, covering both high-level planning and low-level control |
| MeCo: LLM-Empowered Multi-Robot via Memoization | arXiv 2601.20577 | Efficient reuse strategies for multi-robot LLM collaboration |
| CoCoL: Decentralized Collaborative Learning for Multi-Robot | arXiv 2508.20898 | Efficient decentralized collaborative learning for heterogeneous robot systems |
| Retrospective Actor-Critic for Multi-Robot | arXiv 2502.11227 | LLM + reinforcement learning framework for multi-robot collaboration |
| STAR: Multi-Robot Scene Completion (CoRL 2022) | CoRL 2022 | Multi-robot scene completion and collaborative perception |
| DiscoNet: Distilled Collaboration Graph (NeurIPS 2021) | NeurIPS 2021 | Knowledge-distillation-driven multi-agent collaborative perception |
| SyncNet: Latency-Aware Collaborative Perception (ECCV 2022) | ECCV 2022 | Latency-aware inter-device collaborative perception |
| VLMaps: Visual Language Maps (ICRA 2023) | ICRA 2023 | Natural language navigation via VLM features fused with 3D space |
| APEX-MR: Asynchronous Multi-Robot Planning | arXiv 2503.15836 | Asynchronous multi-robot planning and execution framework |

## VIII. Competitive Landscape and Differentiation Analysis

### What Existing Projects Cover:

| Capability Dimension | Existing Projects | Coverage Level |
|----------|----------|--------|
| LLM + Single Device Control | home-llm, Semantic Kernel | Mature |
| Multi-Robot Collaborative Perception | STAR, DiscoNet, SyncNet | Rich academic literature |
| LLM + Multi-Robot Dialogue Collaboration | RoCo, MeCo | Early academic stage |
| IoT Platform + Device Management | ThingsBoard, thin-edge | Mature but lacks LLM integration |
| On-Device LLM Deployment | MLC LLM | Feasible |

### Super IO's Differentiated Positioning (Uncovered Territory):

| Gap Area | Super IO Solution |
|----------|-----------|
| **Semantic Interoperability Among Heterogeneous Devices** | A unified semantic schema that makes lawnmower motor data and camera visual data visible to the LLM at the same semantic layer |
| **LLM as a "Universal Data Bus Translator"** | Not traditional MQTT/Kafka message routing, but LLM-driven semantic-level data fusion |
| **Closed Loop from Data Fusion to Report Generation to Model Iteration** | An integrated "Collection → Fusion → Reporting → Training → Deployment → Collection" full-pipeline system |
| **Real-Time LLM-Dialogue-Based Inter-Device Collaboration** | Not offline batch processing, but real-time streaming collaborative inference among LLMs |
| **Edge + Cloud Heterogeneous LLM Collaborative Architecture** | An architectural design where lightweight edge models perform preprocessing and cloud-based large models perform deep fusion |

---

## IX. Whitepaper Citation Recommendations

### Core Citations (Must-Cite)

1. **RoCo (arXiv 2307.04738)** — Pioneering work on LLM-driven multi-robot collaboration
2. **Home-LLM** (acon96/home-llm) — Best practice for LLM + IoT unified control
3. **VLMaps (ICRA 2023)** — Representative work on VLM for robot spatial understanding
4. **STAR / DiscoNet** — Foundational architecture reference for multi-device collaborative perception
5. **MLC LLM** — Technical foundation for on-device LLM deployment

### Differentiation Narrative Angles

The whitepaper can directly cite the coverage scope of the above projects, then elaborate on Super IO's three core innovations:

1. **Semantic Relay**: Goes beyond transmitting data bytes — the LLM establishes cross-device semantic associations
2. **Liquid Data Bus**: Unlike traditional static schemas, an LLM-empowered adaptive data fusion approach
3. **Lifelong Learning Loop**: Every data fusion and report generation cycle automatically feeds back as model training data

---

> **Document Version**: v1.0-en | **Compilation Date**: 2026-05-30 | **Translator**: Super IO Research Team
> **Source File**: super-io-whitepaper-references.md
> **Translation**: Complete English version, all 21 papers, competitive analysis, and differentiation sections preserved
