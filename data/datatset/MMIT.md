## Multimodal Instruction Tuning Datasets

***Open: whether it is open source,I→ O: Input to Output Modalities, T: Text, I: Image, V: Video, A: Audio,B: Bounding box, 3D: Point Cloud, Tab: Table, and Web: Web page.***

|                         Dataset Name                         |   Open   | Type |       I→O       |   Method    | Multi-Turn |    #.I/V/A     | #.Dialog Turn | #.Instance |
| :----------------------------------------------------------: | :------: | :--: | :-------------: | :---------: | :--------: | :------------: | :-----------: | :--------: |
|         [BuboGPT’s IT](https://bubo-gpt.github.io/)          | &#x2714; | SFT  |   (I+A)/A+T→T   |    Auto.    |  &#x2716;  |    5K/–/9K     |       –       |     9K     |
| [DRESS’s IT](https://huggingface.co/datasets/YangyiYY/LVLM_NLF) | &#x2714; | RLHF |      I+T→T      | Auto.+Manu. |  &#x2714;  |    33K/–/–     |      ∼4       |     –      |
|       [InstructBLIP’s IT](https://llava-vl.github.io/)       | &#x2714; | SFT  |     I/V+T→T     |    Auto.    |  &#x2716;  |       –        |       –       |   ∼ 1.6M   |
|           [LLaVA’s IT](https://llavar.github.io/)            | &#x2714; | SFT  |      I+T→T      |    Auto.    |  &#x2714;  |    81K/–/–     |     2.29      |    150K    |
|         [LLaVA-RLHF](https://llava-rlhf.github.io/)          | &#x2714; | RLHF |      I+T→T      |    Manu.    |  &#x2716;  |     –/–/–      |       –       |    10K     |
|             [LAMM](https://openlamm.github.io/)              | &#x2714; | SFT  |    I+3D+T→T     | Auto.+Manu. |  &#x2714;  |    91K/–/–     |     3.27      |    196K    |
|           [LLaVAR’s IT](https://llavar.github.io/)           | &#x2714; | SFT  |      I+T→T      | LLaVA+Auto. |  &#x2714;  |    20K/–/–     |     2.27      |    174K    |
|         [MIMIC-IT](https://github.com/Luodian/otter)         | &#x2714; | SFT  |     I/V+T→T     |    Auto.    |  &#x2716;  |  8.1M/502K/–   |       1       |    2.8M    |
|          [MGVLID](https://arxiv.org/abs/2307.09474)          |          | SFT  |     I+B+T→T     | Auto.+Manu. |  &#x2716;  |    108K/–/–    |       –       |    108K    |
| [M3 IT](https://huggingface.co/datasets/MMInstruction/M3IT)  | &#x2714; | SFT  |    I/V/B+T→T    | Auto.+Manu. |  &#x2716;  |     –/–/–      |       1       |    2.4M    |
|   [mPLUG-DocOwl’s IT](https://github.com/X-PLUG/mPLUG-Owl)   |          | SFT  |  I/Tab/Web+T→T  |   Inherit   |  &#x2716;  |       –        |       –       |     –      |
|        [MiniGPT-4’s IT](https://minigpt-4.github.io/)        | &#x2714; | SFT  |      I+T→T      |    Auto.    |  &#x2716;  |    134M/–/–    |       1       |     5K     |
|        [MosIT](https://github.com/NExT-GPT/NExT-GPT)         | &#x2714; | SFT  | I+V+A+T→I+V+A+T | Auto.+Manu. |  &#x2714;  |    4K/4K/4K    |      4.8      |     5K     |
|          [MMViG](https://arxiv.org/abs/1608.00272)           |          | RLHF |      I+T→T      |    Manu.    |  &#x2716;  |    16K/–/–     |       –       |    16K     |
|     [Osprey’s IT](https://github.com/CircleRadon/Osprey)     | &#x2714; | SFT  |      I+T→T      | Auto.+Manu. |  &#x2714;  |     –/–/–      |      ∼4       |    724K    |
|        [PandaGPT’s IT](https://panda-gpt.github.io/)         | &#x2714; | SFT  |      I+T→T      |   Inherit   |  &#x2714;  |    81K/–/–     |     2.29      |    160K    |
|       [RLHF-V’s IT](https://github.com/RLHF-V/RLHF-V)        | &#x2714; | RLHF |      I+T→T      |    Manu.    |  &#x2716;  |     –/–/–      |       –       |    1.4K    |
|          [RTVLM](https://arxiv.org/abs/2401.12915)           |          | RLHF |      I+T→T      | Auto.+Manu. |  &#x2716;  |     –/–/–      |       –       |     5K     |
| [StableLLaVA](https://icoz69.github.io/stablellava-official/) | &#x2714; | SFT  |      I+T→T      | Auto.+Manu. |  &#x2716;  |    126K/–/–    |       1       |    126K    |
|       [ShareGPT4V’s IT](https://sharegpt4v.github.io/)       | &#x2714; | SFT  |      I+T→T      | Auto.+Manu. |  &#x2716;  |    100K/–/–    |       –       |     –      |
| [SVIT](https://github.com/BAAI-DCAI/Visual-Instruction-Tuning) | &#x2714; | SFT  |      I+T→T      |    Auto.    |  &#x2714;  |    108K/–/–    |       5       |    3.2M    |
|              [T2M](https://next-gpt.github.io/)              | &#x2714; | SFT  |    T→I/V/A+T    |    Auto.    |  &#x2716;  | 4.9K/4.9K/4.9K |       1       |   14.7K    |
| [VideoChat’s IT](https://github.com/OpenGVLab/Ask-Anything)  | &#x2714; | SFT  |      V+T→T      |    Auto.    |  &#x2714;  |     –/8K/–     |     1.82      |    11K     |
| [Video-LLaMA’s IT](https://github.com/DAMO-NLP-SG/Video-LLaMA) | &#x2714; | SFT  |     I/V+T→T     |    Auto.    |  &#x2714;  |    81K/8K/–    |     2.22      |    171K    |
|         [VLFeedback](https://vlf-silkie.github.io/)          | &#x2714; | RLHF |      I+T→T      |    Auto.    |  &#x2716;  |     –/–/–      |       –       |    80K     |
|      [VLGuard’s IT](https://github.com/ys-zong/VLGuard)      | &#x2714; | RLHF |      I+T→T      |    Auto.    |  &#x2716;  |     3K/–/–     |       –       |     3K     |
| [Video-ChatGPT’s IT](https://github.com/mbzuai-oryx/Video-ChatGPT) | &#x2714; | SFT  |      V+T→T      |   Inherit   |  &#x2714;  |    –/100K/–    |       1       |    100K    |
|   [X-InstructBLIP’s IT](https://arxiv.org/abs/2311.18799)    |          | SFT  |  I/V/A/3D+T→T   |    Auto.    |  &#x2716;  |       –        |       –       |   ∼ 1.8M   |
