# Awesome Papers on Evaluating LLMs and Agents for Scientific R&D

This repository contains a curated list of papers on evaluating LLMs and agents for scientific research and development. It is maintained by [Ziru Chen](https://github.com/ronch99) and will be regularly updated.

## General Scientific R&D

| **Paper**         | **Num of Eval Examples** | **R&D Tasks**         | **Source**                    | **Ecological Validity** | **Contamination Risk** | **Human Performance** | **Time Horizon** |
|-------------------|--------------------------|-----------------------|-------------------------------|-------------------------|------------------------|-----------------------|------------------|
| Discovery Bench    | 239 (Real) / 903 (Synth)       | Code Generation       | Publications                  | N/A                     | Medium                 | N/A                   | -              |
| SciCode           | 80                             | Code Generation       | Publications                  | Expert Validated        | Low                    | N/A                   | -              |
| BLADE             | 12                             | Code Generation       | Publications                  | Expert Validated        | Medium                 | N/A                   | -              |
| ScienceAgent Bench | 102                            | Code Generation       | Publications                  | Expert Validated        | Low                    | N/A                   | 2.5-3h           |
| OpenD5            | 675                            | Hypothesis Generation | Publications, Courses, Kaggle | N/A                     | Medium                 | N/A                   | -              |

- DiscoveryBench (Majumder et al., 2024): Derive data-driven discovery hypothesis for a given research goal/question by generating workflows and programs to analyze data.
- SciCode (Tian et al., 2024): Write code functions based on scientific knowledge and reasoning to perform corresponding scientific compuation tasks.
- BLADE (Gu et al., 2024): Compose a data analysis report for the given research question containing conceptual variables, data transformations, and statistical modeling.
- ScienceAgentBench (Chen et al., 2024): Generate stand-alone programs for solving data-driven discovery tasks, including data processing, model development, data analysis, and information visualization.
- OpenD5 (Zhong et al., 2023): Propose a natural language hypothesis based on a given corpus pair to address the given discovery goal.


## Artificial Intelligence and Data Science

| **Paper**        | **Num of Evaluation Examples** | **R&D Tasks**   | **Source**           | **Ecological Validity** | **Contamination Risk** | **Human Performance** | **Time Horizon** |
|------------------|--------------------------------|-----------------|----------------------|-------------------------|------------------------|-----------------------|------------------|
| MLAgentBench     | 13                             | Code Generation | Kaggle               | N/A                     | Medium                 | N/A                   | -                |
| MLE-Bench        | 75                             | Code Generation | Kaggle               | N/A                     | Medium                 | N/A                   | -                |
| RE-Bench         | 7                              | Code Generation | Created From Scratch | Expert Curation         | Low                    | Yes                   | 8h               |
| DSBench          | 540                            | Code Generation | Kaggle               | N/A                     | High                   | N/A                   | -                |
| DA-Code          | 500                            | Code Generation | Kaggle, Github, Web  | N/A                     | Medium                 | N/A                   | -                |
| Si et al., 2024  |                                | Idea Generation |                      |                         |                        |                       |                  |
| Review Critique  |                                | Paper Reviewing |                      |                         |                        |                       |                  |
| The AI Scientist |                                | R&D Workflow    |                      |                         |                        |                       |                  |
| MLR-copilot      |                                | R&D Workflow    |                      |                         |                        |                       |                  |
| AAAR-1.0         |                                | R&D Workflow    |                      |                         |                        |                       |                  |


## Full Bibliography

- Jun Shern Chan, Neil Chowdhury, Oliver Jaffe, James Aung, Dane Sherburn, Evan Mays, Giulio Starace, Kevin Liu, Leon Maksin, Tejal Patwardhan, Lilian Weng, Aleksander Mądry. 2024. **MLE-bench: Evaluating Machine Learning Agents on Machine Learning Engineering**. In *arXiv*. https://arxiv.org/abs/2410.07095
- Ziru Chen, Shijie Chen, Yuting Ning, Qianheng Zhang, Boshi Wang, Botao Yu, Yifei Li, Zeyi Liao, Chen Wei, Zitong Lu, Vishal Dey, Mingyi Xue, Frazier N. Baker, Benjamin Burns, Daniel Adu-Ampratwum, Xuhui Huang, Xia Ning, Song Gao, Yu Su, Huan Sun. 2024. **ScienceAgentBench: Toward Rigorous Assessment of Language Agents for Data-Driven Scientific Discovery**. In *arXiv*. https://arxiv.org/abs/2410.05080
- Jiangshu Du, Yibo Wang, Wenting Zhao, Zhongfen Deng, Shuaiqi Liu, Renze Lou, Henry Peng Zou, Pranav Narayanan Venkit, Nan Zhang, Mukund Srinath, Haoran Ranran Zhang, Vipul Gupta, Yinghui Li, Tao Li, Fei Wang, Qin Liu, Tianlin Liu, Pengzhi Gao, Congying Xia, Chen Xing, Jiayang Cheng, Zhaowei Wang, Ying Su, Raj Sanjay Shah, Ruohao Guo, Jing Gu, Haoran Li, Kangda Wei, Zihao Wang, Lu Cheng, Surangika Ranathunga, Meng Fang, Jie Fu, Fei Liu, Ruihong Huang, Eduardo Blanco, Yixin Cao, Rui Zhang, Philip S. Yu, Wenpeng Yin. 2024. **LLMs Assist NLP Researchers: Critique Paper (Meta-)Reviewing**. In *EMNLP 2024*. https://arxiv.org/abs/2406.16253
- Ken Gu, Ruoxi Shang, Ruien Jiang, Keying Kuang, Richard-John Lin, Donghe Lyu, Yue Mao, Youran Pan, Teng Wu, Jiaqian Yu, Yikun Zhang, Tianmai M. Zhang, Lanyi Zhu, Mike A. Merrill, Jeffrey Heer, Tim Althoff. **BLADE: Benchmarking Language Model Agents for Data-Driven Science**. In *arXiv*. https://arxiv.org/abs/2408.09667
- Qian Huang, Jian Vora, Percy Liang, Jure Leskovec. 2024. **MLAgentBench: Evaluating Language Agents on Machine Learning Experimentation**. In *ICML 2024*. https://arxiv.org/abs/2310.03302
- Yiming Huang, Jianwen Luo, Yan Yu, Yitong Zhang, Fangyu Lei, Yifan Wei, Shizhu He, Lifu Huang, Xiao Liu, Jun Zhao, Kang Liu. 2024. **DA-Code: Agent Data Science Code Generation Benchmark for Large Language Models**. In *EMNLP 2024*. https://arxiv.org/abs/2410.07331
- Bodhisattwa Prasad Majumder, Harshit Surana, Dhruv Agarwal, Bhavana Dalvi Mishra, Abhijeetsingh Meena, Aryan Prakhar, Tirth Vora, Tushar Khot, Ashish Sabharwal, Peter Clark. **DiscoveryBench: Towards Data-Driven Discovery with Large Language Models**. In *arXiv*. https://arxiv.org/abs/2407.01725
- Liqiang Jing, Zhehui Huang, Xiaoyang Wang, Wenlin Yao, Wenhao Yu, Kaixin Ma, Hongming Zhang, Xinya Du, Dong Yu. 2024. **DSBench: How Far Are Data Science Agents to Becoming Data Science Experts?**. In *arXiv*. https://arxiv.org/abs/2409.07703
- Ruochen Li, Teerth Patel, Qingyun Wang, Xinya Du. 2024. **MLR-Copilot: Autonomous Machine Learning Research based on Large Language Models Agents**. In *arXiv*. https://arxiv.org/abs/2408.14033
- Renze Lou, Hanzi Xu, Sijia Wang, Jiangshu Du, Ryo Kamoi, Xiaoxin Lu, Jian Xie, Yuxuan Sun, Yusen Zhang, Jihyun Janice Ahn, Hongchao Fang, Zhuoyang Zou, Wenchao Ma, Xi Li, Kai Zhang, Congying Xia, Lifu Huang, Wenpeng Yin. 2024. **AAAR-1.0: Assessing AI's Potential to Assist Research**. In *arXiv*. https://arxiv.org/abs/2410.22394
- Chris Lu, Cong Lu, Robert Tjarko Lange, Jakob Foerster, Jeff Clune, David Ha. 2024. **The AI Scientist: Towards Fully Automated Open-Ended Scientific Discovery**. In *arXiv*. https://arxiv.org/abs/2408.06292
- Chenglei Si, Diyi Yang, Tatsunori Hashimoto. 2024. **Can LLMs Generate Novel Research Ideas? A Large-Scale Human Study with 100+ NLP Researchers**. In *arXiv*. https://arxiv.org/abs/2409.04109
- Minyang Tian, Luyu Gao, Shizhuo Dylan Zhang, Xinan Chen, Cunwei Fan, Xuefei Guo, Roland Haas, Pan Ji, Kittithat Krongchon, Yao Li, Shengyan Liu, Di Luo, Yutao Ma, Hao Tong, Kha Trinh, Chenyu Tian, Zihan Wang, Bohao Wu, Yanyu Xiong, Shengzhu Yin, Minhui Zhu, Kilian Lieret, Yanxin Lu, Genglin Liu, Yufeng Du, Tianhua Tao, Ofir Press, Jamie Callan, Eliu Huerta, Hao Peng. **SciCode: A Research Coding Benchmark Curated by Scientists**. In *arXiv*. https://arxiv.org/abs/2407.13168
- Hjalmar Wijk, Tao Lin, Joel Becker, Sami Jawhar, Neev Parikh, Thomas Broadley, Lawrence Chan, Michael Chen, Josh Clymer, Jai Dhyani, Elena Ericheva, Katharyn Garcia, Brian Goodrich, Nikola Jurkovic, Megan Kinniment, Aron Lajko, Seraphina Nix, Lucas Sato, William Saunders, Maksym Taran, Ben West, Elizabeth Barnes. 2024. 
**RE-Bench: Evaluating frontier AI R&D capabilities of language model agents against human experts**. In *arXiv*. https://arxiv.org/abs/2411.15114
- Ruiqi Zhong, Peter Zhang, Steve Li, Jinwoo Ahn, Dan Klein, Jacob Steinhardt. 2023. 
**Goal Driven Discovery of Distributional Differences via Language Descriptions**. In *NeurIPS 2023*. https://arxiv.org/abs/2302.14233