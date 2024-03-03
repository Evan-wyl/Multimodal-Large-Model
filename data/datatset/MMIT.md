## Multimodal Instruction Tuning Datasets

I→ O: Input to Output Modalities, T: Text, I: Image, V: Video, A: Audio,B: Bounding box, 3D: Point Cloud, Tab: Table, and Web: Web page.

|                         Dataset Name                         | Type |       I→O       |   Method    | ***\*Multi-Turn\**** | #.I/V/A        | #.Dialog Turn | #.Instance |
| :----------------------------------------------------------: | :--: | :-------------: | :---------: | -------------------- | -------------- | ------------- | ---------- |
|        [MiniGPT-4’s IT](https://minigpt-4.github.io/)        | SFT  |      I+T→T      |    Auto.    | x                    | 134M/–/–       | 1             | 5K         |
| [StableLLaVA](https://icoz69.github.io/stablellava-official/) | SFT  |      I+T→T      | Auto.+Manu. | x                    | 126K/–/–       | 1             | 126K       |
|           [LLaVA’s IT](https://llavar.github.io/)            | SFT  |      I+T→T      |    Auto.    | Ⅴ                    | 81K/–/–        | 2.29          | 150K       |
| [SVIT](https://github.com/BAAI-DCAI/Visual-Instruction-Tuning) | SFT  |      I+T→T      |    Auto.    | Ⅴ                    | 108K/–/–       | 5             | 3.2M       |
|           [LLaVAR’s IT](https://llavar.github.io/)           | SFT  |      I+T→T      | LLaVA+Auto. | Ⅴ                    | 20K/–/–        | 2.27          | 174K       |
|       [ShareGPT4V’s IT](https://sharegpt4v.github.io/)       | SFT  |      I+T→T      | Auto.+Manu. | x                    | 100K/–/–       | –             | –          |
| [DRESS’s IT](https://huggingface.co/datasets/YangyiYY/LVLM_NLF) | SFT  |      I+T→T      | Auto.+Manu. | Ⅴ                    | 193K/–/–       | ∼4            | –          |
| [VideoChat’s IT](https://github.com/OpenGVLab/Ask-Anything)  | SFT  |      V+T→T      |    Auto.    | Ⅴ                    | –/8K/–         | 1.82          | 11K        |
| [Video-ChatGPT’s IT](https://github.com/mbzuai-oryx/Video-ChatGPT) | SFT  |      V+T→T      |   Inherit   | Ⅴ                    | –/100K/–       | 1             | 100K       |
| [Video-LLaMA’s IT](https://github.com/DAMO-NLP-SG/Video-LLaMA) | SFT  |     I/V+T→T     |    Auto.    | Ⅴ                    | 81K/8K/–       | 2.22          | 171K       |
|       [InstructBLIP’s IT](https://llava-vl.github.io/)       | SFT  |     I/V+T→T     |    Auto.    | x                    | –              | –             | ∼ 1.6M     |
|   [X-InstructBLIP’s IT](https://arxiv.org/abs/2311.18799)    | SFT  |  I/V/A/3D+T→T   |    Auto.    | x                    | –              | –             | ∼ 1.8M     |
|         [MIMIC-IT](https://github.com/Luodian/otter)         | SFT  |     I/V+T→T     |    Auto.    | x                    | 8.1M/502K/–    | 1             | 2.8M       |
|        [PandaGPT’s IT](https://panda-gpt.github.io/)         | SFT  |      I+T→T      |   Inherit   | Ⅴ                    | 81K/–/–        | 2.29          | 160K       |
|          [MGVLID](https://arxiv.org/abs/2307.09474)          | SFT  |     I+B+T→T     | Auto.+Manu. | x                    | 108K/–/–       | –             | 108K       |
| [M3 IT](https://huggingface.co/datasets/MMInstruction/M3IT)  | SFT  |    I/V/B+T→T    | Auto.+Manu. | x                    | –/–/–          | 1             | 2.4M       |
|             [LAMM](https://openlamm.github.io/)              | SFT  |    I+3D+T→T     | Auto.+Manu. | Ⅴ                    | 91K/–/–        | 3.27          | 196K       |
|         [BuboGPT’s IT](https://bubo-gpt.github.io/)          | SFT  |   (I+A)/A+T→T   |    Auto.    | x                    | 5K/–/9K        | –             | 9K         |
|   [mPLUG-DocOwl’s IT](https://github.com/X-PLUG/mPLUG-Owl)   | SFT  |  I/Tab/Web+T→T  |   Inherit   | x                    | –              | –             | –          |
|              [T2M](https://next-gpt.github.io/)              | SFT  |    T→I/V/A+T    |    Auto.    | x                    | 4.9K/4.9K/4.9K | 1             | 14.7K      |
|        [MosIT](https://github.com/NExT-GPT/NExT-GPT)         | SFT  | I+V+A+T→I+V+A+T | Auto.+Manu. | Ⅴ                    | 4K/4K/4K       | 4.8           | 5K         |
|     [Osprey’s IT](https://github.com/CircleRadon/Osprey)     | SFT  |      I+T→T      | Auto.+Manu. | Ⅴ                    | –/–/–          | ∼4            | 724K       |
|         [LLaVA-RLHF](https://llava-rlhf.github.io/)          | RLHF |      I+T→T      |    Manu.    | x                    | –/–/–          | –             | 10K        |
| [DRESS’s IT](https://huggingface.co/datasets/YangyiYY/LVLM_NLF) | RLHF |      I+T→T      | Auto.+Manu. | Ⅴ                    | 33K/–/–        | ∼4            | –          |
|       [RLHF-V’s IT](https://github.com/RLHF-V/RLHF-V)        | RLHF |      I+T→T      |    Manu.    | x                    | –/–/–          | –             | 1.4K       |
|         [VLFeedback](https://vlf-silkie.github.io/)          | RLHF |      I+T→T      |    Auto.    | x                    | –/–/–          | –             | 80K        |
|          [RTVLM](https://arxiv.org/abs/2401.12915)           | RLHF |      I+T→T      | Auto.+Manu. | x                    | –/–/–          | –             | 5K         |
|      [VLGuard’s IT](https://github.com/ys-zong/VLGuard)      | RLHF |      I+T→T      |    Auto.    | x                    | 3K/–/–         | –             | 3K         |
|          [MMViG](https://arxiv.org/abs/1608.00272)           | RLHF |      I+T→T      |    Manu.    | x                    | 16K/–/–        | –             | 16K        |
