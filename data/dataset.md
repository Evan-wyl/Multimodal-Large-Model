## Multimodal Pre-training Datasets

|      Dataset Name      | X Modality  |           #.X            |  #.T  |       #.X-T       | Feat |
| :--------------------: | :---------: | :----------------------: | :---: | :---------------: | :--: |
|         ALIGN          |    Image    |           1.8B           | 1.8B  |       1.8B        |      |
|          LTIP          |    Image    |           312M           | 312M  |       312M        |      |
|        MS-COCO         |    Image    |           124K           | 620K  |       620K        |      |
|     Visual Genome      |    Image    |           108K           | 4.5M  |       4.5M        |      |
|          CC3M          |    Image    |           3.3M           | 3.3M  |       3.3M        |      |
|         CC12M          |    Image    |          12.4M           | 12.4M |       12.4M       |      |
|          SBU           |    Image    |            1M            |  1M   |        1M         |      |
|        LAION-5B        |    Image    |           5.9B           | 5.9B  |       5.9B        |      |
|       LAION-400M       |    Image    |           400M           | 400M  |       400M        |      |
|        LAION-en        |    Image    |           2.3B           | 2.3B  |       2.3B        |      |
|        LAION-zh        |    Image    |           142M           | 142M  |       142M        |      |
|       LAION-COCO       |    Image    |           600M           | 600M  |       600M        |      |
|       Flickr30k        |    Image    |           31K            |  31K  |        31K        |      |
| AI Challenger Captions |    Image    |           300K           | 1.5M  |       1.5M        |      |
|          COYO          |    Image    |           747M           | 747M  |       747M        |      |
|         Wukong         |    Image    |           101M           | 101M  |       101M        |      |
|      COCO Caption      |    Image    |           164K           |  1M   |        1M         |      |
|         WebLI          |    Image    |           10B            |  12B  |        12B        |      |
|     Episodic WebLI     |    Image    |           400M           | 400M  |       400M        |      |
|         CC595k         |    Image    |           595K           | 595K  |       595K        |      |
|        RefCOCO         |    Image    |           20K            | 142K  |       142K        |      |
|        RefCOCO+        |    Image    |           20K            | 142K  |       142K        |      |
|       Visual-7W        |    Image    |          47.3K           | 328K  |       328K        |      |
|        OCR-VQA         |    Image    |           207K           |  1M   |        1M         |      |
|         ST-VQA         |    Image    |           23K            |  32K  |        32K        |      |
|         DocVQA         |    Image    |           12K            |  50K  |        50K        |      |
|        TextVQA         |    Image    |          28.4K           | 45.3K |       45.3K       |      |
|        DataComp        |    Image    |           1.4B           | 1.4B  |       1.4B        |      |
|          GQA           |    Image    |           113K           |  22M  |        22M        |      |
|          VGQA          |    Image    |           108K           | 1.7M  |       1.7M        |      |
|         VQA-v2         |    Image    |           265K           | 1.4M  |       1.4M        |      |
|          DVQA          |    Image    |           300K           | 3.5M  |       3.5M        |      |
|         OK-VQA         |    Image    |           14K            |  14K  |        14K        |      |
|        A-OKVQA         |    Image    |          23.7K           | 24.9K |       24.9K       |      |
|     Text Captions      |    Image    |           28K            | 145K  |       145K        |      |
|    M3W(Interleaved)    |    Image    |           185M           | 182G  | 43.3M(Instances)  |      |
|   MMC4(Interleaved)    |    Image    |           571M           |  43B  | 101.2M(Instances) |      |
|  Obelics(Interleaved)  |    Image    |           353M           | 115M  |  141M(Instances)  |      |
|         MSRVTT         |    Video    |           10K            | 200K  |       200K        |      |
|         WebVid         |    Video    |           10M            |  10M  |        10M        |      |
|          VTP           |    Video    |           27M            |  27M  |        27M        |      |
|       AISHELL-1        |    Audio    |            -             |   -   |       128K        |      |
|       AISHELL-2        |    Audio    |            -             |   -   |        1M         |      |
|        WaveCaps        |    Audio    |           403K           | 403K  |       403K        |      |
|       VSDial-CN        | Image,Audio | 120K(Image), 1.2M(Audio) | 120K  |       1.2M        |      |

**#.X** represents the quantity of X, **#.T** represents the quantity of Text,and **#.X-T** represents the quantity of X-Text pairs, where X can be Image, Video, or Audio.



## Multimodal Instruction Tuning Datasets

| Dataset Name        | Type | I→O                            | Source                                                       | Method      | Multi-Turn | #.I/V/A        | #.Dialog Turn | #.Instance |
| ------------------- | ---- | ------------------------------ | ------------------------------------------------------------ | ----------- | ---------- | -------------- | ------------- | ---------- |
| MiniGPT-4’s IT      | SFT  | I+T→T                          | I+T→T                                                        | CC3M, CC12M | Auto.      | x              | 134M/–/–      | 1          |
| StableLLaVA         | SFT  | I+T→TI+T→T                     | SD (Rombach et al., 2022)                                    | Auto.+Manu. | x          | 126K/–/–       | 1             | 126K       |
| LLaVA’s IT          | SFT  | I+T→TI+T→T                     | MS-COCO                                                      | Auto.       | Ⅴ          | 81K/–/–        | 2.29          | 150K       |
| SVIT                | SFT  | I+T→TI+T→T                     | MS-COCO, Visual Genome                                       | Auto.       | Ⅴ          | 108K/–/–       | 5             | 3.2M       |
| LLaVAR’s IT         | SFT  | I+T→TI+T→T                     | MS-COCO, CC3M, LAION                                         | LLaVA+Auto. | Ⅴ          | 20K/–/–        | 2.27          | 174K       |
| ShareGPT4V’s IT     | SFT  | I+T→TI+T→T                     | LCS, COCO, SAM, TextCaps, WikiArt                            | Auto.+Manu. | x          | 100K/–/–       | –             | –          |
| DRESS’s IT          | SFT  | I+T→TI+T→T                     | LLaVA’s IT, VLSafe                                           | Auto.+Manu. | Ⅴ          | 193K/–/–       | ∼4            | –          |
| VideoChat’s IT      | SFT  | V+T→TV+T→T                     | WebVid                                                       | Auto.       | Ⅴ          | –/8K/–         | 1.82          | 11K        |
| Video-ChatGPT’s IT  | SFT  | V+T→TV+T→T                     | ActivityNet (Caba Heilbron et al., 2015)                     | Inherit     | Ⅴ          | –/100K/–       | 1             | 100K       |
| Video-LLaMA’s IT    | SFT  | I/V+T→TI/V+T→T                 | MiniGPT-4, LLaVA, and VideoChat’s IT                         | Auto.       | Ⅴ          | 81K/8K/–       | 2.22          | 171K       |
| InstructBLIP’s IT   | SFT  | I/V+T→TI/V+T→T                 | Multiple (InstructBLIP’s Figure 2)                           | Auto.       | x          | –              | –             | ∼ 1.6M     |
| X-InstructBLIP’s IT | SFT  | I/V/A/3D+T→TI/V/A/3D+T→T       | Multiple (X-InstructBLIP’s Figure 4)                         | Auto.       | x          | –              | –             | ∼ 1.8M     |
| MIMIC-IT            | SFT  | I/V+T→TI/V+T→T                 | Multiple                                                     | Auto.       | x          | 8.1M/502K/–    | 1             | 2.8M       |
| PandaGPT’s IT       | SFT  | I+T→TI+T→T                     | MiniGPT-4 and LLaVA’s IT                                     | Inherit     | Ⅴ          | 81K/–/–        | 2.29          | 160K       |
| MGVLID              | SFT  | I+B+T→TI+B+T→T                 | Multiple                                                     | Auto.+Manu. | x          | 108K/–/–       | –             | 108K       |
| M3 IT               | SFT  | I/V/B+T→TI/V/B+T→T             | Multiple                                                     | Auto.+Manu. | x          | –/–/–          | 1             | 2.4M       |
| LAMM                | SFT  | I+3D+T→TI+3D+T→T               | Multiple                                                     | Auto.+Manu. | Ⅴ          | 91K/–/–        | 3.27          | 196K       |
| BuboGPT’s IT        | SFT  | (I+A)/A+T→T(I+A)/A+T→T         | Clotho, VGGSS                                                | Auto.       | x          | 5K/–/9K        | –             | 9K         |
| mPLUG-DocOwl’s IT   | SFT  | I/Tab/Web+T→TI/Tab/Web+T→T     | Multiple                                                     | Inherit     | x          | –              | –             | –          |
| T2M                 | SFT  | T→I/V/A+TT→I/V/A+T             | WebVid, CC3M,AudioCap                                        | Auto.       | x          | 4.9K/4.9K/4.9K | 1             | 14.7K      |
| MosIT               | SFT  | I+V+A+T→I+V+A+TI+V+A+T→I+V+A+T | Youtube, Google, Flickr30k, Midjourney, etc.                 | Auto.+Manu. | Ⅴ          | 4K/4K/4K       | 4.8           | 5K         |
| Osprey’s IT         | SFT  | I+T→TI+T→T                     | MS-COCO, RefCOCO, RefCOCO+, LLaVA’s IT etc. (fine-grained region-text dataset) | Auto.+Manu. | Ⅴ          | –/–/–          | ∼4            | 724K       |
| LLaVA-RLHF          | RLHF | I+T→TI+T→T                     | Collected human preference                                   | Manu.       | x          | –/–/–          | –             | 10K        |
| DRESS’s IT          | RLHF | I+T→TI+T→T                     | LLaVA’s IT, VLSafe                                           | Auto.+Manu. | Ⅴ          | 33K/–/–        | ∼4            | –          |
| RLHF-V’s IT         | RLHF | I+T→TI+T→T                     | Collected human preference                                   | Manu.       | x          | –/–/–          | –             | 1.4K       |
| VLFeedback          | RLHF | I+T→TI+T→T                     | Responses generated by 12 MM-LLMs                            | Auto.       | x          | –/–/–          | –             | 80K        |
| RTVLM               | RLHF | I+T→TI+T→T                     | New question-image pairs based on publicly available images  or originally diffusion-generated images (Gallegos et al. 2023), | Auto.+Manu. | x          | –/–/–          | –             | 5K         |
| VLGuard’s IT        | RLHF | I+T→TI+T→T                     | Source image data from various datasets                      | Auto.       | x          | 3K/–/–         | –             | 3K         |
| MMViG               | RLHF | I+T→TI+T→T                     | MS-COCO                                                      | Manu.       | x          | 16K/–/–        | –             | 16K        |

I→ O: Input to Output Modalities, T: Text, I: Image, V: Video, A: Audio,B: Bounding box, 3D: Point Cloud, Tab: Table, and Web: Web page.
