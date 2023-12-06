# A Survey on Multimodal Large Language Models for Autonomous Driving (WACV 2024 LLVM-AD)

## Abstract
With the emergence of Large Language Models (LLMs) and Vision Foundation Models (VFMs), multimodal AI systems benefiting from large models have the potential to equally perceive the real world, make decisions, and control tools as humans. In recent months, LLMs have shown widespread attention in autonomous driving and map systems. Despite its immense potential, there is still a lack of a comprehensive understanding of key challenges, opportunities, and future endeavors to apply in LLM driving systems. In this repo, we present a systematic investigation in this field. We first introduce the background of Multimodal Large Language Models (MLLMs), the multimodal models development using LLMs, and the history of autonomous driving. Then, we overview existing MLLM tools for driving, transportation, and map systems together with existing datasets and benchmarks. Moreover, we summarized the works in The 1st WACV Workshop on Large Language and Vision Models for Autonomous Driving (LLVM-AD), which is the first workshop of its kind regarding LLMs in autonomous driving. To further promote the development of this field, we also discuss several important problems regarding using MLLMs in autonomous driving systems that need to be solved by both academia and industry.      


## Awesome Papers

### MLLM for Perception & Planning & Control for Autonomous Driving

| Model                           | Year | Backbone               | Task              | Modality          | Learning | Input           | Output               |
|---------------------------------|------|------------------------|-------------------|-------------------|----------|-----------------|----------------------|
| [Driving with LLMs](https://arxiv.org/abs/2310.01957)           | 2023 | LLaMA                  | Perception Control| Vector Language   | FT       | Vector Query    | Response \ Actions   |
| [Talk2BEV](https://arxiv.org/abs/2310.02251)                    | 2023 | Flan5XXL Vicuna-13b    | Perception Planning| Vision Language   | ICL      | Image Query     | Response             |
| [GAIA-1](https://arxiv.org/abs/2309.17080)                     | 2023 | -                      | Planning          | Vision Language   | PT       | Video Prompt    | Video                |
| [LMaZP](https://arxiv.org/abs/2201.07207)                       | 2022 | GPT-3 Codex            | Planning          | Language          | ICL      | Text            | Plan                 |
| [Dilu](https://arxiv.org/abs/2309.16292)                        | 2023 | GPT-3.5 GPT-4          | Planning Control  | Language          | ICL      | Text            | Action               |
| [DaYS](https://arxiv.org/abs/2309.10228)                        | 2023 | GPT-4                  | Planning          | Language          | ICL      | Text            | Code                 |
| [RRR](https://arxiv.org/abs/2310.08034)                         | 2023 | GPT-4                  | Planning Control  | Language          | ICL      | Text            | Action               |
| [DlaH](https://arxiv.org/abs/2307.07162)                        | 2023 | GPT-3.5                | Planning Control  | Language          | ICL      | Text            | Action               |
| [GPT-Driver](https://arxiv.org/abs/2310.01415)                  | 2023 | GPT-3.5                | Planning          | Vision Language   | ICL      | Text            | Trajectory           |
| [SurrealDriver](https://arxiv.org/abs/2309.13193)             | 2023 | GPT-4                  | Planning Control  | Language          | ICL      | Text            | Text \ Actions       |
| [LanguageMPC](https://arxiv.org/abs/2310.03026)                | 2023 | GPT-3.5                | Planning          | Language          | ICL      | Text            | Action               |
| [DriveGPT4](https://arxiv.org/abs/2310.01412)                  | 2023 | Llama 2                | Planning Control  | Vision Language   | ICL      | Image Text Action| Text \ Actions       |


### Datasets   
The table is inspired by Comparison and stats in DriveLM    

| Dataset  |    Base Dataset    |    Language Form    |   Perspectives  |   Scale      |  Release?  |
|:---------:|:-------------:|:-------------:|:------:|:--------------------------------------------:|:----------:|
| [BDD-X 2018](https://github.com/JinkyuKimUCB/explainable-deep-driving)  |  [BDD](https://bdd-data.berkeley.edu/)  | Description | Planning Description & Justification    | 8M frames, 20k text strings   |**:heavy_check_mark:**|
| [HAD HRI Advice 2019](https://usa.honda-ri.com/had)  |  [HDD](https://usa.honda-ri.com/hdd)  | Advice | Goal-oriented & stimulus-driven advice | 5,675 video clips, 45k text strings   |**:heavy_check_mark:**|
| [Talk2Car 2019](https://github.com/talk2car/Talk2Car)   |      [nuScenes](https://www.nuscenes.org/)    | Description |  Goal Point Description | 30k frames, 10k text strings | **:heavy_check_mark:**|
| [SUTD-TrafficQA 2021](https://github.com/sutdcv/SUTD-TrafficQA)   |      -    | QA |  QA | 10k frames 62k text strings | **:heavy_check_mark:**|
| [DRAMA 2022](https://usa.honda-ri.com/drama)   |  - | Description |  QA + Captions | 18k frames, 100k text strings | **:heavy_check_mark:**|
| [nuScenes-QA 2023](https://arxiv.org/abs/2305.14836)   |   [nuScenes](https://www.nuscenes.org/)  | QA |  Perception Result     | 30k frames, 460k generated QA pairs| **:heavy_check_mark:** |
| [DriveLM 2023](https://github.com/OpenDriveLab/DriveLM) | [nuScenes](https://www.nuscenes.org/) | QA + Scene Description | Perception, Prediction and Planning with Logic | 30k frames, 360k annotated QA pairs |**:heavy_check_mark:** |
| [MAPLM 2023](https://github.com/LLVM-AD/MAPLM) | [THMA](https://dl.acm.org/doi/10.1609/aaai.v37i13.26848) | QA + Scene Description | Perception, Prediction and HD Map Annotation | 2M frames, 16M annotated HD map Description + 13K released QA pairs | **:heavy_check_mark:** |


## Papers Accept in WACV 2024 LLVM-AD    

Drive as You Speak: Enabling Human-Like Interaction with Large Language Models in Autonomous Vehicles      

Drive Like a Human: Rethinking Autonomous Driving with Large Language Models      

A Game of Bundle Adjustment - Learning Efficient Convergence      

VLAAD: Vision and Language Assistant for Autonomous Driving      

A Safer Vision-based Autonomous Planning System for Quadrotor UAVs with Dynamic Obstacle Trajectory Prediction and Its Application with LLMs     

Human-Centric Autonomous Systems With LLMs for User Command Reasoning      

NuScenes-MQA: Integrated Evaluation of Captions and QA for Autonomous Driving Datasets using Markup Annotations       

Latency Driven Spatially Sparse Optimization for Multi-Branch CNNs for Semantic Segmentation       

LIP-Loc: LiDAR Image Pretraining for Cross-Modal Localization      

## Citation    

If the survey and our workshop inspire you, please cite our work:    

```
@misc{cui2023survey,
      title={A Survey on Multimodal Large Language Models for Autonomous Driving}, 
      author={Can Cui and Yunsheng Ma and Xu Cao and Wenqian Ye and Yang Zhou and Kaizhao Liang and Jintai Chen and Juanwu Lu and Zichong Yang and Kuei-Da Liao and Tianren Gao and Erlong Li and Kun Tang and Zhipeng Cao and Tong Zhou and Ao Liu and Xinrui Yan and Shuqi Mei and Jianguo Cao and Ziran Wang and Chao Zheng},
      year={2023},
      eprint={2311.12320},
      archivePrefix={arXiv},
      primaryClass={cs.AI}
}
```


