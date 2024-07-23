# VLM Dreamer
CLIPを報酬モデルとして用いることで自然言語を介して強化学習のタスクを指定できるようにするという開発

## 概略図
<img src="https://github.com/user-attachments/assets/b6abd3d5-131c-41e6-9c42-b1716c48b881" width=400px>

アーキテクチャ: [Vision-Language Models are Zero-Shot Reward Models for Reinforcement Learning](https://arxiv.org/abs/2310.12921)

RLアルゴリズム: [Dreamer](https://arxiv.org/abs/1912.01603)

## 現状の性能
行動指示用プロンプト: "a humanoid robot kneeling"

<img src="https://github.com/twin1shun/VLM-Dreamer/assets/128522258/86478278-2056-49e2-a372-80acea943243" width=400px>

## 工夫点
1. 既存研究 ([Vision-Language Models are Zero-Shot Reward Models for Reinforcement Learning](https://arxiv.org/abs/2310.12921)) で使われていたRLアルゴリズムを"Soft Actor Critic"から"Dreamer"に変更した。
2. ドメイン汎化能力の高いCLIPを得るために [Improving Zero-Shot Generalization for CLIP with Synthesized Prompts](https://arxiv.org/abs/2307.07397) に基づいて [UCF101](https://www.crcv.ucf.edu/data/UCF101.php) で学習させた。
3. colabで実験しやすいように既存研究のコードを.pyファイルから.ipynbファイルに書き直した。
