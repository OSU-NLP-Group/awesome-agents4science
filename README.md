# Awesome Papers on Evaluating LLMs and Agents for Scientific R&D

Abstract

## Table of Contents

x

## Multi-Disciplinary

| **Paper**         | **Num of Eval Examples** | **R&D Tasks**         | **Source**                    | **Ecological Validity** | **Contamination Risk** | **Human Performance** | **Time Horizon** |
|-------------------|--------------------------|-----------------------|-------------------------------|-------------------------|------------------------|-----------------------|------------------|
| Discovery Bench    | 239 (Real) / 903 (Synth)       | Code Generation       | Publications                  | N/A                     | Medium                 | N/A                   | N/A              |
| SciCode           | 80                             | Code Generation       | Publications                  | Expert Validated        | Low                    | N/A                   | N/A              |
| BLADE             | 12                             | Code Generation       | Publications                  | Expert Validated        | Medium                 | N/A                   | N/A              |
| ScienceAgent Bench | 102                            | Code Generation       | Publications                  | Expert Validated        | Low                    | N/A                   | 2.5-3h           |
| OpenD5            | 675                            | Hypothesis Generation | Publications, Courses, Kaggle | N/A                     | Medium                 | N/A                   | N/A              |


- DiscoveryBench (Majumder et al., 2024): Derive data-driven discovery hypothesis for a given research goal/question by generating workflows and programs to analyze data.
- SciCode (Tian et al., 2024): Write code functions based on scientific knowledge and reasoning to perform corresponding scientific compuation tasks.
- BLADE (Gu et al., 2024): Compose a data analysis report for the given research question containing conceptual variables, data transformations, and statistical modeling.
- ScienceAgentBench (Chen et al., 2024): Generate stand-alone programs for solving data-driven discovery tasks, including data processing, model development, data analysis, and information visualization.
- OpenD5 (Zhong et al., 2023): Propose a natural language hypothesis based on a given corpus pair to address the given discovery goal.

## Machine Learning and Data Science

| **Paper**        | **Num of Evaluation Examples** | **R&D Tasks**   | **Source**           | **Ecological Validity** | **Contamination Risk** | **Human Performance** | **Time Horizon** |
|------------------|--------------------------------|-----------------|----------------------|-------------------------|------------------------|-----------------------|------------------|
| MLAgentBench     | 13                             | Code Generation | Kaggle               |                         |                        |                       |                  |
| MLE-Bench        | 75                             | Code Generation | Kaggle               |                         |                        |                       |                  |
| RE-Bench         | 7                              | Code Generation | Created From Scratch |                         |                        |                       |                  |
| DSBench          | 540                            | Code Generation | Kaggle               |                         |                        |                       |                  |
| DA-Code          | 500                            | Code Generation | Kaggle, Github, Web  |                         |                        |                       |                  |
| Si et al., 2024  |                                | Idea Generation |                      |                         |                        |                       |                  |
| Review Critique  |                                | Paper Reviewing |                      |                         |                        |                       |                  |
| The AI Scientist |                                | R&D Workflow    |                      |                         |                        |                       |                  |
| MLR-copilot      |                                | R&D Workflow    |                      |                         |                        |                       |                  |
| AAAR-1.0         |                                | R&D Workflow    |                      |                         |                        |                       |                  |


## Full Bibliography

- Ziru Chen, Shijie Chen, Yuting Ning, Qianheng Zhang, Boshi Wang, Botao Yu, Yifei Li, Zeyi Liao, Chen Wei, Zitong Lu, Vishal Dey, Mingyi Xue, Frazier N. Baker, Benjamin Burns, Daniel Adu-Ampratwum, Xuhui Huang, Xia Ning, Song Gao, Yu Su, Huan Sun. 2024. ScienceAgentBench: Toward Rigorous Assessment of Language Agents for Data-Driven Scientific Discovery. In *arXiv*. https://arxiv.org/abs/2410.05080
- Ken Gu, Ruoxi Shang, Ruien Jiang, Keying Kuang, Richard-John Lin, Donghe Lyu, Yue Mao, Youran Pan, Teng Wu, Jiaqian Yu, Yikun Zhang, Tianmai M. Zhang, Lanyi Zhu, Mike A. Merrill, Jeffrey Heer, Tim Althoff. BLADE: Benchmarking Language Model Agents for Data-Driven Science. In *arXiv*. https://arxiv.org/abs/2408.09667
- Bodhisattwa Prasad Majumder, Harshit Surana, Dhruv Agarwal, Bhavana Dalvi Mishra, Abhijeetsingh Meena, Aryan Prakhar, Tirth Vora, Tushar Khot, Ashish Sabharwal, Peter Clark. DiscoveryBench: Towards Data-Driven Discovery with Large Language Models. In *arXiv*. https://arxiv.org/abs/2407.01725
- Minyang Tian, Luyu Gao, Shizhuo Dylan Zhang, Xinan Chen, Cunwei Fan, Xuefei Guo, Roland Haas, Pan Ji, Kittithat Krongchon, Yao Li, Shengyan Liu, Di Luo, Yutao Ma, Hao Tong, Kha Trinh, Chenyu Tian, Zihan Wang, Bohao Wu, Yanyu Xiong, Shengzhu Yin, Minhui Zhu, Kilian Lieret, Yanxin Lu, Genglin Liu, Yufeng Du, Tianhua Tao, Ofir Press, Jamie Callan, Eliu Huerta, Hao Peng. SciCode: A Research Coding Benchmark Curated by Scientists. In *arXiv*. https://arxiv.org/abs/2407.13168
- Ruiqi Zhong, Peter Zhang, Steve Li, Jinwoo Ahn, Dan Klein, Jacob Steinhardt. 2023. 
Goal Driven Discovery of Distributional Differences via Language Descriptions. In *NeurIPS 2023*. https://arxiv.org/abs/2302.14233