# Awesome Papers on Agents for Science

This repository contains a curated list of papers on evaluating LLMs and agents for scientific research and development. It is maintained by [Ziru Chen](https://github.com/ronch99) and will be regularly updated.

## Table of Contents
- [Benchmarks and Evaluation](#benchmarks-and-evaluation)
- [Agents for Science](#agents-for-science)
    - [Machine Learning and Data Science](#machine-learning-and-data-science)
    - [Biology and Medicine](#biology-and-medicine)
    - [Chemistry and Material Science](#chemistry-and-material-science)
    - [Other Disciplines](#other-disciplines)
    - [Task-Specific Agents](#task-specific-agents)
- [Opinions and Prospectives](#opinions-and-prospectives)
- [Full Bibliography](#full-bibliography)

## Benchmarks and Evaluation

| **Paper**          | **R&D Tasks**         | **Scientific Domains**                                                                                           | **Num of Evaluation Examples** | **Source**                    | **Ecological Validity**$^*$ | **Contamination Risk** | **Human Performance** | **Time Horizon** |
|--------------------|-----------------------|------------------------------------------------------------------------------------------------------------------|--------------------------------|-------------------------------|-------------------------|------------------------|-----------------------|------------------|
| [Discovery Bench](https://arxiv.org/abs/2407.01725) | Code Generation       | Sociology, Biology, Economics, Engineering, Meta-science, Humanities                                             | 239 (Real) / 903 (Synth)       | Publications                  | N/A                     | Medium                 | N/A                   | -                |
| [SciCode](https://arxiv.org/abs/2407.13168)         | Code Generation       | Mathematics, Physics, Biology, Chemistry, Material Science                                                       | 80                             | Publications                  | Expert Validated        | Low                    | N/A                   | -                |
| [BLADE](https://arxiv.org/abs/2408.09667)          | Code Generation       | Behavioral Sciences, Finance and Economics, Demographics, Education, Health and Well-being, Evolutionary Biology | 12                             | Publications                  | Expert Validated        | Medium                 | N/A                   | -                |
| [ScienceAgent Bench](https://arxiv.org/abs/2410.05080) | Code Generation       | Bioinformatics, Computational Chemistry, Geographical Information Science, Psychology and Cognitive NeuroScience | 102                            | Publications                  | Expert Validated        | Low                    | N/A                   | 2.5-3h           |
| [MLAgentBench](https://arxiv.org/abs/2310.03302)   | Code Generation       | Machine Learning                                                                                                 | 13                             | Kaggle, Recent Research       | N/A                     | Medium                 | N/A                   | -                |
| [MLE-Bench](https://arxiv.org/abs/2410.07095)      | Code Generation       | Machine Learning                                                                                                 | 75                             | Kaggle                        | N/A                     | Medium                 | N/A                   | -                |
| [RE-Bench](https://arxiv.org/abs/2411.15114)       | Code Generation       | Machine Learning                                                                                                 | 7                              | Created From Scratch          | Expert Curation         | Low                    | Yes                   | 8h               |
| [DSBench](https://arxiv.org/abs/2409.07703)        | Code Generation       | Data Science                                                                                                     | 540                            | Eloquence, Kaggle             | N/A                     | High                   | N/A                   | -                |
| [DA-Code](https://arxiv.org/abs/2410.07331)        | Code Generation       | Data Science                                                                                                     | 500                            | Kaggle, Github, Web           | N/A                     | Medium                 | N/A                   | -                |
| [CHIME](https://arxiv.org/abs/2404.02831)          | Literature Review     | Biomedicine                                                                                                      | 472 (100 expert annotated)     | Publications                  | Subset Expert Validated | Low                    | N/A                   | -                |
| [Qi et al., 2023](https://arxiv.org/abs/2402.13225) | Hypothesis Generation | Biomedicine                                                                                                       | 200                            | Publications                  | N/A                     | Low                    | N/A                   | -                |
| [OpenD5](https://arxiv.org/abs/2406.16253)         | Hypothesis Generation | Business, Social Sciences, Humanities, Health, Machine Learning                                                  | 675                            | Publications, Courses, Kaggle | N/A                     | Medium                 | N/A                   | -                |
| [ReviewCritique](https://arxiv.org/abs/2406.16253)       | Reviewing & Meta-Reviewing | Natural Language Processing                                                                                          | 100 papers and corresponding reviews | Publications, OpenReview | Expert Annotated        | Low                    | N/A                   | -                |
| [AAAR-1.0](https://arxiv.org/abs/2410.22394)       | R&D Workflow          | Artificial Intelligence                                                                                          | 1049 (Equation Inference) 100 (Experiment Design) 993 (Paper Weakness) 11,376 (Review Critique) | Publications, OpenReview | Expert Validated        | High                    | N/A                   | -                |

<p align="center">
$^*$ Ecological validity refers to how well the results of a study can be applied to real-world situations.
</p>

- **DiscoveryBench (Majumder et al., 2024)**: Derive data-driven discovery hypothesis for a given research goal/question by generating workflows and programs to analyze data.

- **SciCode (Tian et al., 2024)**: Write code functions based on scientific knowledge and reasoning to perform corresponding scientific compuation tasks.

- **BLADE (Gu et al., 2024)**: Compose a data analysis report for the given research question containing conceptual variables, data transformations, and statistical modeling.

- **ScienceAgentBench (Chen et al., 2024)**: Generate stand-alone programs for solving data-driven discovery tasks, including data processing, model development, data analysis, and information visualization.

- **MLAgentBench (Huang et al., 2024a)**: Edit programs in a given workspace, which also contains the dataset needed, to complete the specified machine learning problem. 

- **MLE-Bench (Chan et al., 2024)**: Train machine learning models to maximize their performance on adapted Kaggle challenges.

- **RE-Bench (Wijk et al., 2024)**: Compare LLM-based agents' performance against human experts on machine learning R&D tasks in the same programming environment.

- **DSBench (Jing et al., 2024)**: Answer data analysis or modeling questions by writing programs to derive the solutions.

- **DA-Code (Huang et al., 2024b)**: Write Python programs and SQL queries to solve complex Data Science tasks, including data wrangling, machine learning, and so on.

- **CHIME (Hsu et al., 2024)**: Produce hierarchical organizations of scientific studies to assist researchers with literature review. 

- **Qi el al. (2023)**: Propose hypothesis in biomedical research based on instruction and background knowledge. 

- **OpenD5 (Zhong et al., 2023)**: Propose a natural language hypothesis based on a given corpus pair to address the given discovery goal.

- **AAAR-1.0 (Lou at al., 2024)**: Evaluate large language models on four tasks in R&D workflow: assess correctness of equations based on context, design experiments to validate research ideas and solutions, identify weaknesses in paper submissions, and identify whether each segment in human reviews is deficient or not.

- **ReviewCritique (Du et al., 2024)**: Examine LLMs ability to assist in paper (meta-)reviewing and its recognizability.  


## Agents for Science

### Machine Learning and Data Science
- **The AI Scientist (Lu et al., 2024)**: A comprehensive framework that enables large language models to autonomously conduct scientific research in machine learning, encompassing tasks from idea generation to executing experiments and authoring full scientific papers.

- **MLR-Copilot (Li et al., 2024b)**: An agent framework that leverages large language model agents to autonomously generate and implement research ideas, aiming to enhance productivity in machine learning research.

### Biology and Medicine
- **ProtAgents (Ghafarollahi and Buehler, 2024b)**: A multi-agent AI framework using Large Language Models (LLMs) to collaboratively design de novo proteins by combining physics-based simulations and machine learning for complex problem-solving.

- **TAIS (Liu et al., 2024)**: A framework that utilizes large language models to automate the scientific discovery process by simulating roles such as project manager, data engineer, and domain expert, aiming to identify disease-predictive genes from gene expression data.

- **BioDiscoveryAgent (Roohani, et al., 2024)**: An AI agent that leverages large language models to design genetic perturbation experiments, demonstrating significant improvements over traditional methods in identifying genes linked to specific phenotypes.

- **Gao et al. (2024)**: The paper envisions "AI scientists" as collaborative agents that integrate AI models with experimental platforms to enhance biomedical research by combining human expertise with AI's data analysis capabilities. 

- **AgentMD (Jin et al., 2024a)**: A language agent capable of automatically curating and applying clinical calculators, significantly improving risk prediction accuracy and clinical workflows.

- **DrugAgent (Inoue et al., 2024)**: A multi-agent framework that leverages machine learning and knowledge integration to enhance drug repurposing by training robust drug-target interaction models, extracting data from various biomedical databases, and validating predictions through literature analysis. 

- **MedAgents (Tang et al., 2024a)**: A framework where large language models (LLMs) assume specialized roles and engage in collaborative, multi-round discussions to enhance zero-shot medical reasoning without additional training. 

### Chemistry and Material Science
- **Chemist-X (Chen et al., 2023)**: An AI agent leveraging retrieval-augmented generation (RAG) and large language models (LLMs) to automate reaction condition recommendations in chemical synthesis, bridging the gap between computational tools and chemical research.

- **Coscientist (Boiko et al., 2023)**: An agent system combining large language models to autonomously plan, design, and execute scientific experiments, demonstrating its capabilities through successful catalyzed chemical reactions while addressing safety concerns and proposing misuse prevention measures.

- **ChemCrow (Bran et al., 2024)**: A large-language model agent that integrates 18 expert-designed tools to enhance performance in tasks such as organic synthesis, drug discovery, and materials design. 

- **ChatMOF (Kang and Kim, 2023)**: An autonomous AI system that utilizes large-scale language models to predict and generate metal-organic frameworks (MOFs) by extracting key details from textual inputs and managing tasks such as data retrieval, property prediction, and structure generation.

- **ChatGPT Research Group (Zheng et al., 2023)**: A dynamic AI-driven laboratory ecosystem that integrates multiple AI assistants to automate and optimize the synthesis of metal-organic frameworks (MOFs) and covalent organic frameworks (COFs), thereby enhancing their crystallinity through minimal human intervention.

### Other Disciplines
- **AtomAgents (Ghafarollahi and Buehler, 2024a)**: A physics-aware generative AI platform that leverages the collaborative capabilities of multiple AI agents, including large language models, to autonomously design metallic alloys with enhanced properties by integrating knowledge retrieval, multi-modal data analysis, and physics-based simulations. 

- **Mephisto (Sun et al., 2024)**: A multi-agent framework leveraging large language models to emulate human reasoning in interpreting multi-band galaxy observations, achieving near-human proficiency in analyzing data from the James Webb Space Telescope, including newly identified "Little Red Dot" galaxies.

- **Ning et al. (2024)**: The paper proposes an autonomous GIS agent framework that retrieves geospatial data by generating, executing, and debugging programs, enabling flexible and extensible integration of various data sources.

- **GIS Copilot (Akinboyewa et al., 2024)**: A framework that integrates Large Language Models (LLMs) into existing Geographic Information System (GIS) platforms, exemplified by QGIS, to autonomously generate spatial analysis workflows and code, thereby enabling users to perform spatial analyses through natural language commands. 

### Task-Specific Agents
- **VirSci (Su et al., 2024)**: A large language model-based multi-agent system that emulates collaborative scientific research to enhance the generation of novel and impactful scientific ideas.

- **AgentReview (Jin et al., 2024b)**: A large language model-based framework that simulates peer review processes, uncovering biases and sociological dynamics like social influence, altruism fatigue, and authority bias to improve review mechanisms.

- **PaperQA2 (Skarlinski et al., 2024)**: A language model agent optimized for factual accuracy, which matches or surpasses subject matter experts in literature search tasks, including information retrieval, summarization, and contradiction detection. 

- **ResearchAgent (Baek et al., 2024)**: A large language model-powered system that autonomously generates and refines research ideas—encompassing problems, methods, and experimental designs—by analyzing scientific literature and incorporating feedback from multiple reviewing agents. 

- **CoI agent (Li et al., 2024a)**: An LLM-based system that organizes relevant literature into a sequential structure to emulate the progressive development within a research domain, thereby enhancing the generation of novel research ideas. 


## Opinions and Prospectives
- **Tang et al. (2024b)**: The paper examines the potential risks associated with large language model (LLM)-based agents in scientific research, proposing a triadic safeguarding framework involving human regulation, agent alignment, and agent regulation to mitigate these vulnerabilities.

- **Messeri and Crockett (2024)**: The paper examines how the integration of artificial intelligence (AI) in scientific research may lead to overestimations of understanding, potentially fostering uniformity in methodologies and diminishing scientific innovation.

- **Morris (2023)**: The paper examines scientists' views on how generative AI could enhance various aspects of their work, including research, education, and communication, while also addressing potential concerns.


## Full Bibliography

- Temitope Akinboyewa, Zhenlong Li, Huan Ning, M. Naser Lessani. 2024. **GIS Copilot: Towards an Autonomous GIS Agent for Spatial Analysis**. In *arXiv*. https://arxiv.org/abs/2411.03205 

- Jinheon Baek, Sujay Kumar Jauhar, Silviu Cucerzan, Sung Ju Hwang. 2024. **ResearchAgent: Iterative Research Idea Generation over Scientific Literature with Large Language Models**. In *arXiv*. https://arxiv.org/abs/2404.07738 

- Daniil A. Boiko, Robert MacKnight, Gabe Gomes. 2023. **Autonomous chemical research with large language models**. In *Nature*. https://doi.org/10.1038/s41586-023-06792-0

- Andres M. Bran, Sam Cox, Oliver Schilter, Carlo Baldassari, Andrew D. White, Philippe Schwaller. 2024. **Augmenting large language models with chemistry tools**. In *Nat Mach Intell*. https://doi.org/10.1038/s42256-024-00832-8 

- Jun Shern Chan, Neil Chowdhury, Oliver Jaffe, James Aung, Dane Sherburn, Evan Mays, Giulio Starace, Kevin Liu, Leon Maksin, Tejal Patwardhan, Lilian Weng, Aleksander Mądry. 2024. **MLE-bench: Evaluating Machine Learning Agents on Machine Learning Engineering**. In *arXiv*. https://arxiv.org/abs/2410.07095

- Kexin Chen, Junyou Li, Kunyi Wang, Yuyang Du, Jiahui Yu, Jiamin Lu, Lanqing Li, Jiezhong Qiu, Jianzhang Pan, Yi Huang, Qun Fang, Pheng Ann Heng, Guangyong Chen. 2023. **Chemist-X: Large Language Model-empowered Agent for Reaction Condition Recommendation in Chemical Synthesis**. In *arXiv*. https://arxiv.org/abs/2311.10776

- Ziru Chen, Shijie Chen, Yuting Ning, Qianheng Zhang, Boshi Wang, Botao Yu, Yifei Li, Zeyi Liao, Chen Wei, Zitong Lu, Vishal Dey, Mingyi Xue, Frazier N. Baker, Benjamin Burns, Daniel Adu-Ampratwum, Xuhui Huang, Xia Ning, Song Gao, Yu Su, Huan Sun. 2024. **ScienceAgentBench: Toward Rigorous Assessment of Language Agents for Data-Driven Scientific Discovery**. In *arXiv*. https://arxiv.org/abs/2410.05080

- Jiangshu Du, Yibo Wang, Wenting Zhao, Zhongfen Deng, Shuaiqi Liu, Renze Lou, Henry Peng Zou, Pranav Narayanan Venkit, Nan Zhang, Mukund Srinath, Haoran Ranran Zhang, Vipul Gupta, Yinghui Li, Tao Li, Fei Wang, Qin Liu, Tianlin Liu, Pengzhi Gao, Congying Xia, Chen Xing, Jiayang Cheng, Zhaowei Wang, Ying Su, Raj Sanjay Shah, Ruohao Guo, Jing Gu, Haoran Li, Kangda Wei, Zihao Wang, Lu Cheng, Surangika Ranathunga, Meng Fang, Jie Fu, Fei Liu, Ruihong Huang, Eduardo Blanco, Yixin Cao, Rui Zhang, Philip S. Yu, Wenpeng Yin. 2024. **LLMs Assist NLP Researchers: Critique Paper (Meta-)Reviewing**. In *EMNLP 2024*. https://arxiv.org/abs/2406.16253

- Shanghua Gao, Ada Fang, Yepeng Huang, Valentina Giunchiglia, Ayush Noori, Jonathan Richard Schwarz, Yasha Ektefaie, Jovana Kondic, Marinka Zitnik. 2024. **Empowering Biomedical Discovery with AI Agents**. In *arXiv*. https://arxiv.org/abs/2404.02831

- Alireza Ghafarollahi, Markus J. Buehler. 2024a. **AtomAgents: Alloy design and discovery through physics-aware multi-modal multi-agent artificial intelligence**. In *arXiv*. https://arxiv.org/abs/2407.10022 

- Alireza Ghafarollahi, Markus J. Buehler. 2024b. **ProtAgents: Protein discovery via large language model multi-agent collaborations combining physics and machine learning**. In *arXiv*. https://arxiv.org/abs/2402.04268

- Ken Gu, Ruoxi Shang, Ruien Jiang, Keying Kuang, Richard-John Lin, Donghe Lyu, Yue Mao, Youran Pan, Teng Wu, Jiaqian Yu, Yikun Zhang, Tianmai M. Zhang, Lanyi Zhu, Mike A. Merrill, Jeffrey Heer, Tim Althoff. **BLADE: Benchmarking Language Model Agents for Data-Driven Science**. In *arXiv*. https://arxiv.org/abs/2408.09667

- Chao-Chun Hsu, Erin Bransom, Jenna Sparks, Bailey Kuehl, Chenhao Tan, David Wadden, Lucy Lu Wang, and Aakanksha Naik. 2024. **CHIME: LLM-Assisted Hierarchical Organization of Scientific Studies for Literature Review Support**. In *Findings of ACL 2024*. https://arxiv.org/abs/2407.16148

- Qian Huang, Jian Vora, Percy Liang, Jure Leskovec. 2024a. **MLAgentBench: Evaluating Language Agents on Machine Learning Experimentation**. In *ICML 2024*. https://arxiv.org/abs/2310.03302

- Yiming Huang, Jianwen Luo, Yan Yu, Yitong Zhang, Fangyu Lei, Yifan Wei, Shizhu He, Lifu Huang, Xiao Liu, Jun Zhao, Kang Liu. 2024b. **DA-Code: Agent Data Science Code Generation Benchmark for Large Language Models**. In *EMNLP 2024*. https://arxiv.org/abs/2410.07331

- Yoshitaka Inoue, Tianci Song, Tianfan Fu. 2024. **DrugAgent: Explainable Drug Repurposing Agent with Large Language Model-based Reasoning**. In *arXiv*. https://arxiv.org/abs/2408.13378 

- Qiao Jin, Zhizheng Wang, Yifan Yang, Qingqing Zhu, Donald Wright, Thomas Huang, W John Wilbur, Zhe He, Andrew Taylor, Qingyu Chen, Zhiyong Lu. 2024a. **AgentMD: Empowering Language Agents for Risk Prediction with Large-Scale Clinical Tool Learning**. In *arXiv*. https://arxiv.org/abs/2402.13225

- Yiqiao Jin, Qinlin Zhao, Yiyang Wang, Hao Chen, Kaijie Zhu, Yijia Xiao, Jindong Wang. 2024b. **AgentReview: Exploring Peer Review Dynamics with LLM Agents**. In *EMNLP 2024*. https://arxiv.org/abs/2406.12708

- Liqiang Jing, Zhehui Huang, Xiaoyang Wang, Wenlin Yao, Wenhao Yu, Kaixin Ma, Hongming Zhang, Xinya Du, Dong Yu. 2024. **DSBench: How Far Are Data Science Agents to Becoming Data Science Experts?**. In *arXiv*. https://arxiv.org/abs/2409.07703

- Yeonghun Kang, Jihan Kim. 2023. **ChatMOF: An Autonomous AI System for Predicting and Generating Metal-Organic Frameworks**. In *arXiv*. https://arxiv.org/abs/2308.01423 

- Long Li, Weiwen Xu, Jiayan Guo, Ruochen Zhao, Xingxuan Li, Yuqian Yuan, Boqiang Zhang, Yuming Jiang, Yifei Xin, Ronghao Dang, Deli Zhao, Yu Rong, Tian Feng, Lidong Bing. 2024a. **Chain of Ideas: Revolutionizing Research Via Novel Idea Development with LLM Agents**. In *arXiv*. https://arxiv.org/abs/2410.13185 

- Ruochen Li, Teerth Patel, Qingyun Wang, Xinya Du. 2024b. **MLR-Copilot: Autonomous Machine Learning Research based on Large Language Models Agents**. In *arXiv*. https://arxiv.org/abs/2408.14033

- Haoyang Liu, Yijiang Li, Jinglin Jian, Yuxuan Cheng, Jianrong Lu, Shuyi Guo, Jinglei Zhu, Mianchen Zhang, Miantong Zhang, Haohan Wang. 2024. **Toward a Team of AI-made Scientists for Scientific Discovery from Gene Expression Data**. In *arXiv*. https://arxiv.org/abs/2402.12391

- Renze Lou, Hanzi Xu, Sijia Wang, Jiangshu Du, Ryo Kamoi, Xiaoxin Lu, Jian Xie, Yuxuan Sun, Yusen Zhang, Jihyun Janice Ahn, Hongchao Fang, Zhuoyang Zou, Wenchao Ma, Xi Li, Kai Zhang, Congying Xia, Lifu Huang, Wenpeng Yin. 2024. **AAAR-1.0: Assessing AI's Potential to Assist Research**. In *arXiv*. https://arxiv.org/abs/2410.22394

- Chris Lu, Cong Lu, Robert Tjarko Lange, Jakob Foerster, Jeff Clune, David Ha. 2024. **The AI Scientist: Towards Fully Automated Open-Ended Scientific Discovery**. In *arXiv*. https://arxiv.org/abs/2408.06292

- Bodhisattwa Prasad Majumder, Harshit Surana, Dhruv Agarwal, Bhavana Dalvi Mishra, Abhijeetsingh Meena, Aryan Prakhar, Tirth Vora, Tushar Khot, Ashish Sabharwal, Peter Clark. **DiscoveryBench: Towards Data-Driven Discovery with Large Language Models**. In *arXiv*. https://arxiv.org/abs/2407.01725

- Lisa Messeri, M. J. Crockett. 2024. **Artificial intelligence and illusions of understanding in scientific research**. In *Nature*. https://doi.org/10.1038/s41586-024-07146-0  

- Meredith Ringel Morris. 2023. **Scientists' Perspectives on the Potential for Generative AI in their Fields**. In *arXiv*. https://arxiv.org/abs/2304.01420

- Huan Ning, Zhenlong Li, Temitope Akinboyewa, M. Naser Lessani. 2024. **An Autonomous GIS Agent Framework for Geospatial Data Retrieval**. In *arXiv*. https://arxiv.org/abs/2407.21024

- Biqing Qi, Kaiyan Zhang, Haoxiang Li, Kai Tian, Sihang Zeng, Zhang-Ren Chen, Jin-Fang Hu, Bowen Zhou. 2023. **Large Language Models are Zero Shot Hypothesis Proposers**. In *Instruction Workshop @ NeurIPS 2023*. https://arxiv.org/abs/2311.05965

- Yusuf Roohani, Andrew Lee, Qian Huang, Jian Vora, Zachary Steinhart, Kexin Huang, Alexander Marson, Percy Liang, Jure Leskovec. 2024. **BioDiscoveryAgent: An AI Agent for Designing Genetic Perturbation Experiments**. In *arXiv*. https://arxiv.org/abs/2405.17631

- Chenglei Si, Diyi Yang, Tatsunori Hashimoto. 2024. **Can LLMs Generate Novel Research Ideas? A Large-Scale Human Study with 100+ NLP Researchers**. In *arXiv*. https://arxiv.org/abs/2409.04109

- Michael D. Skarlinski, Sam Cox, Jon M. Laurent, James D. Braza, Michaela Hinks, Michael J. Hammerling, Manvitha Ponnapati, Samuel G. Rodriques, Andrew D. White. 2024. **Language agents achieve superhuman synthesis of scientific knowledge**. In *arXiv*. https://arxiv.org/abs/2409.13740 

- Haoyang Su, Renqi Chen, Shixiang Tang, Xinzhe Zheng, Jingzhe Li, Zhenfei Yin, Wanli Ouyang, Nanqing Dong. 2024. **Two Heads Are Better Than One: A Multi-Agent System Has the Potential to Improve Scientific Idea Generation**. In *arXiv*. https://arxiv.org/abs/2410.09403

- Zechang Sun, Yuan-Sen Ting, Yaobo Liang, Nan Duan, Song Huang, and Zheng Cai. 2024. **Interpreting Multi-band Galaxy Observations with Large Language Model-Based Agents**. In *arXiv*. https://arxiv.org/abs/2409.14807 

- Xiangru Tang, Anni Zou, Zhuosheng Zhang, Ziming Li, Yilun Zhao, Xingyao Zhang, Arman Cohan, and Mark Gerstein. 2024a. **MedAgents: Large Language Models as Collaborators for Zero-shot Medical Reasoning**. In *Findings of ACL 2024*. https://arxiv.org/abs/2311.10537 

- Xiangru Tang, Qiao Jin, Kunlun Zhu, Tongxin Yuan, Yichi Zhang, Wangchunshu Zhou, Meng Qu, Yilun Zhao, Jian Tang, Zhuosheng Zhang, Arman Cohan, Zhiyong Lu, Mark Gerstein. 2024b. **Prioritizing Safeguarding Over Autonomy: Risks of LLM Agents for Science**. In *arXiv*. https://arxiv.org/abs/2402.04247

- Minyang Tian, Luyu Gao, Shizhuo Dylan Zhang, Xinan Chen, Cunwei Fan, Xuefei Guo, Roland Haas, Pan Ji, Kittithat Krongchon, Yao Li, Shengyan Liu, Di Luo, Yutao Ma, Hao Tong, Kha Trinh, Chenyu Tian, Zihan Wang, Bohao Wu, Yanyu Xiong, Shengzhu Yin, Minhui Zhu, Kilian Lieret, Yanxin Lu, Genglin Liu, Yufeng Du, Tianhua Tao, Ofir Press, Jamie Callan, Eliu Huerta, Hao Peng. **SciCode: A Research Coding Benchmark Curated by Scientists**. In *arXiv*. https://arxiv.org/abs/2407.13168

- Hjalmar Wijk, Tao Lin, Joel Becker, Sami Jawhar, Neev Parikh, Thomas Broadley, Lawrence Chan, Michael Chen, Josh Clymer, Jai Dhyani, Elena Ericheva, Katharyn Garcia, Brian Goodrich, Nikola Jurkovic, Megan Kinniment, Aron Lajko, Seraphina Nix, Lucas Sato, William Saunders, Maksym Taran, Ben West, Elizabeth Barnes. 2024. **RE-Bench: Evaluating frontier AI R&D capabilities of language model agents against human experts**. In *arXiv*. https://arxiv.org/abs/2411.15114

- Zhiling Zheng, Oufan Zhang, Ha L. Nguyen, Nakul Rampal, Ali H. Alawadhi, Zichao Rong, Teresa Head-Gordon, Christian Borgs, Jennifer T. Chayes, Omar M. Yaghi. 2023. **ChatGPT Research Group for Optimizing the Crystallinity of MOFs and COFs**. In *ACS Cent Sci*. https://doi.org/10.1021/acscentsci.3c01087

- Ruiqi Zhong, Peter Zhang, Steve Li, Jinwoo Ahn, Dan Klein, Jacob Steinhardt. 2023. 
**Goal Driven Discovery of Distributional Differences via Language Descriptions**. In *NeurIPS 2023*. https://arxiv.org/abs/2302.14233
