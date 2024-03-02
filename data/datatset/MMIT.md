## Multimodal Instruction Tuning Datasets

I→ O: Input to Output Modalities, T: Text, I: Image, V: Video, A: Audio,B: Bounding box, 3D: Point Cloud, Tab: Table, and Web: Web page.

|    Dataset Name     | Type |       I→O       |   Method    | ***\*Multi-Turn\**** | #.I/V/A        | #.Dialog Turn | #.Instance |
| :-----------------: | :--: | :-------------: | :---------: | -------------------- | -------------- | ------------- | ---------- |
|   MiniGPT-4’s IT    | SFT  |      I+T→T      |    Auto.    | x                    | 134M/–/–       | 1             | 5K         |
|     StableLLaVA     | SFT  |      I+T→T      | Auto.+Manu. | x                    | 126K/–/–       | 1             | 126K       |
|     LLaVA’s IT      | SFT  |      I+T→T      |    Auto.    | Ⅴ                    | 81K/–/–        | 2.29          | 150K       |
|        SVIT         | SFT  |      I+T→T      |    Auto.    | Ⅴ                    | 108K/–/–       | 5             | 3.2M       |
|     LLaVAR’s IT     | SFT  |      I+T→T      | LLaVA+Auto. | Ⅴ                    | 20K/–/–        | 2.27          | 174K       |
|   ShareGPT4V’s IT   | SFT  |      I+T→T      | Auto.+Manu. | x                    | 100K/–/–       | –             | –          |
|     DRESS’s IT      | SFT  |      I+T→T      | Auto.+Manu. | Ⅴ                    | 193K/–/–       | ∼4            | –          |
|   VideoChat’s IT    | SFT  |      V+T→T      |    Auto.    | Ⅴ                    | –/8K/–         | 1.82          | 11K        |
| Video-ChatGPT’s IT  | SFT  |      V+T→T      |   Inherit   | Ⅴ                    | –/100K/–       | 1             | 100K       |
|  Video-LLaMA’s IT   | SFT  |     I/V+T→T     |    Auto.    | Ⅴ                    | 81K/8K/–       | 2.22          | 171K       |
|  InstructBLIP’s IT  | SFT  |     I/V+T→T     |    Auto.    | x                    | –              | –             | ∼ 1.6M     |
| X-InstructBLIP’s IT | SFT  |  I/V/A/3D+T→T   |    Auto.    | x                    | –              | –             | ∼ 1.8M     |
|      MIMIC-IT       | SFT  |     I/V+T→T     |    Auto.    | x                    | 8.1M/502K/–    | 1             | 2.8M       |
|    PandaGPT’s IT    | SFT  |      I+T→T      |   Inherit   | Ⅴ                    | 81K/–/–        | 2.29          | 160K       |
|       MGVLID        | SFT  |     I+B+T→T     | Auto.+Manu. | x                    | 108K/–/–       | –             | 108K       |
|        M3 IT        | SFT  |    I/V/B+T→T    | Auto.+Manu. | x                    | –/–/–          | 1             | 2.4M       |
|        LAMM         | SFT  |    I+3D+T→T     | Auto.+Manu. | Ⅴ                    | 91K/–/–        | 3.27          | 196K       |
|    BuboGPT’s IT     | SFT  |   (I+A)/A+T→T   |    Auto.    | x                    | 5K/–/9K        | –             | 9K         |
|  mPLUG-DocOwl’s IT  | SFT  |  I/Tab/Web+T→T  |   Inherit   | x                    | –              | –             | –          |
|         T2M         | SFT  |    T→I/V/A+T    |    Auto.    | x                    | 4.9K/4.9K/4.9K | 1             | 14.7K      |
|        MosIT        | SFT  | I+V+A+T→I+V+A+T | Auto.+Manu. | Ⅴ                    | 4K/4K/4K       | 4.8           | 5K         |
|     Osprey’s IT     | SFT  |      I+T→T      | Auto.+Manu. | Ⅴ                    | –/–/–          | ∼4            | 724K       |
|     LLaVA-RLHF      | RLHF |      I+T→T      |    Manu.    | x                    | –/–/–          | –             | 10K        |
|     DRESS’s IT      | RLHF |      I+T→T      | Auto.+Manu. | Ⅴ                    | 33K/–/–        | ∼4            | –          |
|     RLHF-V’s IT     | RLHF |      I+T→T      |    Manu.    | x                    | –/–/–          | –             | 1.4K       |
|     VLFeedback      | RLHF |      I+T→T      |    Auto.    | x                    | –/–/–          | –             | 80K        |
|        RTVLM        | RLHF |      I+T→T      | Auto.+Manu. | x                    | –/–/–          | –             | 5K         |
|    VLGuard’s IT     | RLHF |      I+T→T      |    Auto.    | x                    | 3K/–/–         | –             | 3K         |
|        MMViG        | RLHF |      I+T→T      |    Manu.    | x                    | 16K/–/–        | –             | 16K        |
