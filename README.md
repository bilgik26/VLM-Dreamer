# VLM Dreamer
アーキテクチャ: [Vision-Language Models are Zero-Shot Reward Models for Reinforcement Learning](https://arxiv.org/abs/2310.12921)

RL アルゴリズム: [Dreamer](https://arxiv.org/abs/1912.01603)

## 現状の性能
行動指示用プロンプト: "a humanoid robot kneeling"

<img src="https://github.com/twin1shun/VLM-Dreamer/assets/128522258/86478278-2056-49e2-a372-80acea943243" width=400px>

## 工夫点
ドメイン汎化能力の高いCLIPを得るために[Improving Zero-Shot Generalization for CLIP with Synthesized Prompts](https://arxiv.org/abs/2307.07397)に基づいて[UCF101](https://www.crcv.ucf.edu/data/UCF101.php)で学習させました
