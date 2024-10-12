# GPT4off
GPT-4off official github
![header](https://capsule-render.vercel.app/api?type=waving&color=auto&height=300&section=header&text=GPT-4off&fontSize=90)

# 0. Getting Started (시작하기)
```bash
$ npm start
```

<br/>
<br/>

# 1. Paper Overview
- Paper
    - GPT-4off : On-Board Traversable Probability Estimation for Off-Road via GPT Knowledge Distillation
- Abstract
    - This paper proposes a framework for predicting traversable probability in off-road environments by distilling knowledge from large language models (LLMs) such as GPT-4o into lightweight models. The GPT-4off approach utilizes GPT-generated data to train a compact model capable of real-time operation on edge devices such as the NVIDIA Orin board. Unlike traditional systems that focus on identifying traversable areas, this study emphasizes predicting traversable probability, facilitating faster decision-making in complex environments. This is particularly advantageous for unmanned ground vehicles (UGVs), where obstacles and terrain variability present significant challenges. The GPT-4off framework enhances real-time performance through knowledge distillation and domain-specific optimization, ensuring efficient resource use while maintaining LLM-level performance. Experimental results on the RUGD off-road dataset show that the lightweight model achieves GPT-level performance while being deployable on edge devices. This framework effectively reduces human annotation costs and RAM power consumption, improving the practicality of off-road autonomous driving systems and demonstrating the potential to leverage LLM capabilities for low-power, real-time applications.
<br/>
<br/>

# 2. Dataset
- RUGD Dataset
    - http://rugd.vision/ 
- Prompt
    - Assume that a military armored vehicle is driving on this path. The armored vehicle can push through all obstacles even without a road, can climb inclines and rough rocks, can pass through small puddles, can move forward without getting stuck in sand, but cannot hit people. \newline Does this photo seem drivable? On a scale of 0\% to 100\%, what would be the percentage of drivable probability? Please write the final drivable probability(\%) in the first line of your answer. Provide three reasons for your estimation for selecting that certain percentage.
- RUGD probaility output
    - RUGD_final.zip

## 5.4 Cooperation
|  |  |
|-----------------|-----------------|
| Git    |  <img src="https://github.com/user-attachments/assets/483abc38-ed4d-487c-b43a-3963b33430e6" alt="git" width="100">    |
| Git Kraken    |  <img src="https://github.com/user-attachments/assets/32c615cb-7bc0-45cd-91ea-0d1450bfc8a9" alt="git kraken" width="100">    |
| Notion    |  <img src="https://github.com/user-attachments/assets/34141eb9-deca-416a-a83f-ff9543cc2f9a" alt="Notion" width="100">    |

<br/>

# 6. File Structure
```plaintext
RUGD_final/
└── label.txt

# label.txt
trail_00051.png	80        # [image_name] [probability percentage(%)]
trail_01761.png	70
...
```

<br/>
<br/>
