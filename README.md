<h1 align="center"> Awesome Table Question Answering </h1>

<p align="center">
  <a href="https://github.com/RenzeLou/awesome-instruction-learning"><img src="https://awesome.re/badge.svg" alt="Awesome" /></a>
</p>

<p align="center">
🔥🔥🔥 An awesome paper list of <b>Table-based Question Answering</b>. 
</p>


## Table of Contents
- [Table of Contents](#table-of-contents)
- [Existing Survey](#existing-survey)
- [Dataset](#dataset)
  - [Single-Turn](#single-turn)
  - [Multiple-Turn](#multiple-turn)
- [Methods](#methods)
  - [Table Pretraining (TaLMs)](#table-pretraining-talms)
  - [LLM-based Methods](#llm-based-methods)
  - [Retrieval-then-Read Methods](#retrieval-then-read-methods)
    - [Multi-hop](#multi-hop)
    - [Numerical Reasoning](#numerical-reasoning)
    - [Open-Domain](#open-domain)
    - [Multimodal Reasoning](#multimodal-reasoning)
  - [Non-Retrieval Methods](#non-retrieval-methods)
  

## Existing Survey

- **A Survey on Table-and-Text HybridQA: Concepts, Methods, Challenges and Future Directions** 2022.12
   
   [[Paper](https://arxiv.org/abs/2212.13465)]*Dingzirui Wang, Longxu Dou, Wanxiang Che*

- **A Survey on Text-to-SQL Parsing: Concepts, Methods, and Future Directions** 2022.08

   [[Paper](https://arxiv.org/pdf/2208.13629.pdf)]*Bowen Qin, Binyuan Hui, Lihan Wang, Min Yang, Jinyang Li, Binhua Li, Ruiying Geng, Rongyu Cao, Jian Sun, Luo Si, Fei Huang, Yongbin Li*

- **A survey on table question answering: recent advances** 2022.07
   
   [[Paper](https://arxiv.org/pdf/2207.05270.pdf)]*Nengzheng Jin, Joanna Siebert, Dongfang Li, Qingcai Chen*

- **A Survey on Neural Data-to-Text Generation** 2023.08

   [[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10215344)]*Yupian Lin, Tong Ruan, Jingping Liu, Haofen Wang*

- **Large Language Model for Table Processing: A Survey** 2024.10  

   [[Paper](https://arxiv.org/abs/2402.05121)] [[Github](https://github.com/godaai/llm-table-survey)] *Weizheng Lu, Jing Zhang, Ju Fan, Zihao Fu, Yueguo Chen, Xiaoyong Du*

- **Paper list on LLMs for table-related tasks**

    [Awesome-Tabular-LLMs](https://github.com/SpursGoZmy/Awesome-Tabular-LLMs)
  
    [LLM-Table-Survey](https://github.com/godaai/llm-table-survey)

## Dataset

### Single-Turn

- **Compositional Semantic Parsing on Semi-Structured Tables** `WikiTableQuestions` 2015
  
    [[Paper](https://arxiv.org/abs/1508.00305)] [[Code](https://ppasupat.github.io/WikiTableQuestions/)] *EPanupong Pasupat, Percy Liang* 
   
- **Seq2SQL: Generating Structured Queries from Natural Language using Reinforcement Learning** `WikiSQL` 2017

    [[Paper](https://arxiv.org/abs/1709.00103)] [[Code](https://github.com/salesforce/WikiSQL)] *Victor Zhong, Caiming Xiong, Richard Socher*

- **Spider: A Large-Scale Human-Labeled Dataset for Complex and Cross-Domain Semantic Parsing and Text-to-SQL Task** `Spider` <ins>EMNLP</ins> 2018

    [[Paper](https://arxiv.org/abs/1809.08887)] [[Code](https://github.com/taoyds/spider)] *Tao Yu, Rui Zhang, Kai Yang, Michihiro Yasunaga, Dongxu Wang, Zifan Li, James Ma, Irene Li, Qingning Yao, Shanelle Roman, Zilin Zhang, Dragomir Radev*

- **On the Potential of Lexico-logical Alignments for Semantic Parsing to SQL Queries** `SQUALL` <ins>EMNLP-Findings</ins> 2020

    [[Paper](https://arxiv.org/abs/2010.11246)] [[Code](https://www.github.com/tzshi/squall)] *Tianze Shi, Chen Zhao, Jordan Boyd-Graber, Hal Daumé III, Lillian Lee*
   
- **HybridQA: A Dataset of Multi-Hop Question Answering over Tabular and Textual Data** `HybridQA` <ins>EMNLP-Findings</ins> 2020
    
    [[Paper](https://aclanthology.org/2020.findings-emnlp.91/)] [[Code](https://github.com/wenhuchen/HybridQA)] *Wenhu Chen, Hanwen Zha, Zhiyu Chen, Wenhan Xiong, Hong Wang, William Yang Wang*

- **ToTTo: A Controlled Table-To-Text Generation Dataset** `ToTTo` <ins>EMNLP</ins> 2020
    
    [[Paper](https://arxiv.org/abs/2004.14373)] [[Code](https://github.com/google-research-datasets/totto)] *Ankur P. Parikh, Xuezhi Wang, Sebastian Gehrmann, Manaal Faruqui, Bhuwan Dhingra, Diyi Yang, Dipanjan Das*

- **TSQA: tabular scenario based question answering** `GeoTSQA` <ins>AAAI</ins> 2021
    
    [[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/17570)] [[Code](https://github.com/nju-websoft/TSQA)] *Xiao Li, Yawei Sun, Gong Cheng*

- **TAT-QA: A Question Answering Benchmark on a Hybrid of Tabular and Textual Content in Finance** `TAT-QA` <ins>ACL</ins> 2021
    
    [[Paper](https://aclanthology.org/2021.acl-long.254/)] [[Code](https://github.com/NExTplusplus/TAT-QA)] *Fengbin Zhu, Wenqiang Lei, Youcheng Huang, Chao Wang, Shuo Zhang, Jiancheng Lv, Fuli Feng, Tat-Seng Chua*

- **Open Domain Question Answering over Tables via Dense Retrieval** `NQ-table` <ins>NAACL</ins> 2021
   
    [[Paper](https://aclanthology.org/2021.naacl-main.43/)] [[Code](https://github.com/google-research/tapas)] *Jonathan Herzig, Thomas Müller, Syrine Krichene, Julian Eisenschlos* 

- **Open Question Answering over Tables and Text** `OTT-QA` <ins>ICLR</ins> 2021
   
    [[Paper](https://arxiv.org/abs/2010.10439)] [[Code](https://github.com/wenhuchen/OTT-QA)] *Wenhu Chen, Ming-Wei Chang, Eva Schlinger, William Wang, William W. Cohen* 

- **MultiModalQA: complex question answering over text, tables and images** `MultimodalQA` <ins>ICLR</ins> 2021
   
    [[Paper](https://openreview.net/forum?id=ee6W5UgQLa)] [[Code](https://github.com/allenai/multimodalqa)] *Alon Talmor, Ori Yoran, Amnon Catav, Dan Lahav, Yizhong Wang, Akari Asai, Gabriel Ilharco, Hannaneh Hajishirzi, Jonathan Berant* 

- **Finqa: A dataset of numerical reasoning over financial data** `FinQA` <ins>EMNLP</ins> 2021
   
    [[Paper](https://arxiv.org/abs/2109.00122)] [[Code](https://github.com/czyssrs/FinQA)] *Zhiyu Chen, Wenhu Chen, Charese Smiley, Sameena Shah, Iana Borova, Dylan Langdon, Reema Moussa, Matt Beane, Ting-Hao Huang, Bryan Routledge, William Yang Wang* 

- **HiTab: A Hierarchical Table Dataset for Question Answering and Natural Language Generation** `HiTab` <ins>ACL</ins> 2022
    
    [[Paper](https://aclanthology.org/2022.acl-long.78/)] [[Code](https://github.com/microsoft/hitab)] *Zhoujun Cheng, Haoyu Dong, Zhiruo Wang, Ran Jia, Jiaqi Guo, Yan Gao, Shi Han, Jian-Guang Lou, Dongmei Zhang*

- **FeTaQA: Free-form Table Question Answering** `FeTaQA` <ins>TACL</ins> 2022
    
    [[Paper](https://aclanthology.org/2022.tacl-1.3/)] [[Code](https://github.com/Yale-LILY/FeTaQA)] *Linyong Nan, Chiachun Hsieh, Ziming Mao, Xi Victoria Lin, Neha Verma, Rui Zhang, Wojciech Kryściński, Hailey Schoelkopf, Riley Kong, Xiangru Tang, Mutethia Mutuma, Ben Rosand, Isabel Trindade, Renusree Bandaru, Jacob Cunningham, Caiming Xiong, Dragomir Radev, Dragomir Radev*

- **MultiHiertt: Numerical Reasoning over Multi Hierarchical Tabular and Textual Data** `MultiHiertt` <ins>ACL</ins> 2022
    
    [[Paper](https://aclanthology.org/2022.acl-long.454)] [[Code](https://github.com/psunlpgroup/MultiHiertt)] *Yilun Zhao, Yunxiang Li, Chenying Li, Rui Zhang*

- **Learning to Imagine: Integrating Counterfactual Thinking in Neural Discrete Reasoning** `TAT-HQA` <ins>ACL</ins> 2022
    
    [[Paper](https://aclanthology.org/2022.acl-long.5.pdf)] *Moxin Li, Fuli Feng, Hanwang Zhang, Xiangnan He, Fengbin Zhu, Tat-Seng Chua*

- **Towards Complex Document Understanding By Discrete Reasoning** `TAT-DQA` <ins>ACM MM</ins> 2022
    
    [[Paper](https://dl.acm.org/doi/abs/10.1145/3503161.3548422)] *Fengbin Zhu, Wenqiang Lei, Fuli Feng, Chao Wang, Haozhou Zhang, Tat-Seng Chua*

- **AIT-QA: Question Answering Dataset over Complex Tables in the Airline Industry** `AIT-QA` <ins>NAACL</ins> 2022
    
    [[Paper](https://aclanthology.org/2022.naacl-industry.34/)] [[Code](https://github.com/IBM/AITQA)] *Yannis Katsis, Saneem Chemmengath, Vishwajeet Kumar, Samarth Bharadwaj, Mustafa Canim, Michael Glass, Alfio Gliozzo, Feifei Pan, Jaydeep Sen, Karthik Sankaranarayanan, Soumen Chakrabarti*

- **Open-WikiTable: Dataset for Open Domain Question Answering with Complex Reasoning over Table** `Open-Wikitable` <ins>ACL-Findings</ins> 2023

    [[Paper](https://arxiv.org/abs/2305.07288)] *Sunjun Kweon, Yeonsu Kwon, Seonhee Cho, Yohan Jo, Edward Choi*



### Multiple-Turn

- **CoQA: A Conversational Question Answering Challenge** `CoQA` <ins>TACL</ins> 2019
    
    [[Paper](https://direct.mit.edu/tacl/article/doi/10.1162/tacl_a_00266/43511/CoQA-A-Conversational-Question-Answering-Challenge)] [[Code](https://stanfordnlp.github.io/coqa)] *Siva Reddy, Danqi Chen, Christopher D. Manning*
    
- **PACIFIC: Towards proactive conversational question answering over tabular and textual data in finance** `Pacific` <ins>EMNLP</ins> 2022
    
    [[Paper](https://arxiv.org/abs/2210.08817)] [[Code](https://github.com/dengyang17/PACIFIC/)] *Yang Deng, Wenqiang Lei, Wenxuan Zhang, Wai Lam, Tat-Seng Chua*

- **ConvFinQA: Exploring the Chain of Numerical Reasoning in Conversational Finance Question Answering** `ConvFinQA` <ins>EMNLP</ins> 2022
    
    [[Paper](https://aclanthology.org/2022.emnlp-main.421/)] [[Code](https://github.com/czyssrs/ConvFinQA)] *Zhiyu Chen, Shiyang Li, Charese Smiley, Zhiqiang Ma, Sameena Shah, William Yang Wang*

- **HybriDialogue: An Information-Seeking Dialogue Dataset Grounded on Tabular and Textual Data** `HybriDialogue` <ins>EMNLP-Findings</ins> 2022
    
    [[Paper](https://aclanthology.org/2022.findings-acl.41/)] [[Code](https://github.com/entitize/HybridDialogue)] *Kai Nakamura, Sharon Levy, Yi-Lin Tuan, Wenhu Chen, William Yang Wang*
   
- **MMCoQA: Conversational Question Answering over Text, Tables, and Images** `MMCoQA` <ins>ACL</ins> 2022
    
    [[Paper](https://aclanthology.org/2022.acl-long.290/)] [[Code](https://github.com/liyongqi67/mmcoqa)] *Yongqi Li, Wenjie Li, Liqiang Nie*



## Methods

### Table Pretraining (TaLMs)

- **TaBERT: Pretraining for Joint Understanding of Textual and Tabular Data**  <ins>ACL</ins> 2020

    `WikiTableQuestions, Spider`

    [[Paper](https://arxiv.org/pdf/2005.08314.pdf)] [[Code](http://fburl.com/TaBERT)] *Pengcheng Yin, Graham Neubig, Wen-tau Yih, Sebastian Riedel*

- **MATE: Multi-view Attention for Table Transformer Efficiency**  <ins>EMNLP</ins> 2021

    `WikiTableQuestions, HybridQA`

    [[Paper](https://arxiv.org/abs/2109.04312)] *Julian Martin Eisenschlos, Maharshi Gor, Thomas Müller, William W. Cohen*

- **TAPEX: Table pre-training via learning a neural SQL executor**  <ins>ICLR</ins> 2022

    `WikiSQL, WikiTableQuestions, SQA`

    [[Paper](https://arxiv.org/pdf/2107.07653.pdf)] [[Code](https://github.com/microsoft/Table-Pretraining)] *Qian Liu, Bei Chen, Jiaqi Guo, Morteza Ziyadi, Zeqi Lin, Weizhu Chen, Jian-Guang Lou*

- **OmniTab: Pretraining with Natural and Synthetic Data for Few-shot Table-based Question Answering**  <ins>NAACL</ins> 2022

    `WikiSQL, WikiTableQuestions`

    [[Paper](https://aclanthology.org/2022.naacl-main.68.pdf)] [[Code](https://github.com/jzbjyb/OmniTab)] *Zhengbao Jiang, Yi Mao, Pengcheng He, Graham Neubig, Weizhu Chen*

- **ReasTAP: Injecting Table Reasoning Skills During Pre-training via Synthetic Reasoning Examples**  <ins>EMNLP</ins> 2022

    `WikiSQL, WikiTableQuestions`

    [[Paper](https://aclanthology.org/2022.naacl-main.68.pdf)] [[Code](https://github.com/Yale-LILY/ReasTAP)] *Yilun Zhao, Linyong Nan, Zhenting Qi, Rui Zhang, Dragomir Radev*




### LLM-based Methods

- **Binding Language Models in Symbolic Languages**  <ins>ICLR</ins> 2023

    `WikiSQL, WikiTableQuestions, MultimodalQA`

    [[Paper](https://arxiv.org/abs/2210.02875)] [[Code](https://lm-code-binder.github.io)]*Zhoujun Cheng, Tianbao Xie, Peng Shi, Chengzu Li, Rahul Nadkarni, Yushi Hu, Caiming Xiong, Dragomir Radev, Mari Ostendorf, Luke Zettlemoyer, Noah A. Smith, Tao Yu*

- **Large Language Models are Versatile Decomposers: Decompose Evidence and Questions for Table-based Reasoning**  <ins>SIGIR</ins> 2023

    `WikiSQL, WikiTableQuestions`

    [[Paper](https://arxiv.org/abs/2301.13808)] *Yunhu Ye, Binyuan Hui, Min Yang, Binhua Li, Fei Huang, Yongbin Li*

- **Large language models are few (1)-shot table reasoners**  <ins>EACL-Findings</ins> 2023

    `WikiTableQuestions, FetaQA`

    [[Paper](https://arxiv.org/abs/2210.06710)] *Wenhu Chen*

- **Program of Thoughts Prompting: Disentangling Computation from Reasoning for Numerical Reasoning Tasks**  <ins>Arxiv</ins> 2023

    `WikiTableQuestions, FetaQA`

    [[Paper](https://arxiv.org/abs/2211.12588)] *Wenhu Chen, Xueguang Ma, Xinyi Wang, William W Cohen*

- **Structgpt: A general framework for large language model to reason over structured data**  <ins>Arxiv</ins> 2023

    `WikiSQL, WikiTableQuestions`

    [[Paper](https://arxiv.org/abs/2305.09645)] *Jinhao Jiang, Kun Zhou, Zican Dong, Keming Ye, Wayne Xin Zhao, Ji-Rong Wen*

- **LEVER: Learning to Verify Language-to-Code Generation with Execution** <ins>ICML</ins> 2023

   `WikiTableQuestions`

   [[Paper](https://proceedings.mlr.press/v202/ni23b/ni23b.pdf)] *Ansong Ni, Srini Iyer, Dragomir Radev, Veselin Stoyanov, Wen-tau Yih, Sida Wang, Xi Victoria Lin*

- **Generate, Transform, Answer: Question Specific Tool Synthesis for Tabular Data** 2023

   `WikiTableQuestions`

   [[Paper](https://arxiv.org/abs/2303.10138)] *Carlos Gemmell, Jeffrey Dalton*


### Retrieval-then-Read Methods

#### Multi-hop

- **MATE: Multi-view Attention for Table Transformer Efficiency**  <ins>EMNLP</ins> 2021

    ` WikiTableQuestions, HybridQA`

    [[Paper](https://arxiv.org/abs/2109.04312)] *Julian Martin Eisenschlos, Maharshi Gor, Thomas Müller, William W. Cohen*

- **Reasoning over hybrid chain for table-and-text open domain question answering** `CARP` <ins>IJCAI</ins> 2022

    `OTT-QA`

    [[Paper](https://www.ijcai.org/proceedings/2022/0629.pdf)] *Wanjun Zhong, Junjie Huang, Qian Liu, Ming Zhou, Jiahai Wang, Jian Yin, Nan Duan*

- **Multi-hop open-domain question answering over structured and unstructured knowledge**  `DEHG` <ins>NAACL-Findings</ins> 2022

    `HybridQA`

    [[Paper](https://aclanthology.org/2022.findings-naacl.12/)] *Yue Feng, Zhen Han, Mingming Sun, Ping Li*

- **Mixed-modality Representation Learning and Pre-training for Joint Table-and-Text Retrieval in OpenQA**  `OTTeR` <ins>EMNLP-Findings</ins> 2022

    `OTT-QA`

    [[Paper](https://arxiv.org/abs/2210.05197)] *Junjie Huang, Wanjun Zhong, Qian Liu, Ming Gong, Daxin Jiang, Nan Duan*

- **MuGER2: Multi-Granularity Evidence Retrieval and Reasoning for Hybrid Question Answering**  `MuGER` <ins>EMNLP-Findings</ins> 2022

    `HybridQA`

    [[Paper](https://arxiv.org/abs/2210.10350)] *Yingyao Wang, Junwei Bao, Chaoqun Duan, Youzheng Wu, Xiaodong He, Tiejun Zhao*

- **TACR: A Table-alignment-based Cell-selection and Reasoning Model for Hybrid Question-Answering**  `TACR` <ins>ACL-Findings</ins> 2023

    `HybridQA`

    [[Paper](https://arxiv.org/abs/2305.14682)] *Jian Wu, Yicheng Xu, Yan Gao, Jian-Guang Lou, Börje F. Karlsson, Manabu Okumura*

- **MAFiD: Moving Average Equipped Fusion-in-Decoder for Question Answering over Tabular and Textual Data**  `MAFiD` <ins>EACL-Findings</ins> 2023

    `HybridQA`

    [[Paper](https://aclanthology.org/2023.findings-eacl.177/)] *Sung-Min Lee, Eunhwan Park, Daeryong Seo, Donghyeon Jeon, Inho Kang, Seung-Hoon Na*

- **S3HQA: A Three-Stage Approach for Multi-hop Text-Table Hybrid Question Answering** `S3HQA` <ins>ACL</ins> 2023

    `HybridQA`

   [[Paper](https://arxiv.org/abs/2305.11725)] *Fangyu Lei, Xiang Li, Yifan Wei, Shizhu He, Yiming Huang, Jun Zhao, Kang Liu*

- **Multi-Row, Multi-Span Distant Supervision For Table+Text Question Answering**  `MITQA` <ins>ACL</ins> 2023

    `HybridQA, OTT-QA`

    [[Paper](https://aclanthology.org/2023.acl-long.449/)] *Vishwajeet Kumar, Yash Gupta, Saneem Chemmengath, Jaydeep Sen, Soumen Chakrabarti, Samarth Bharadwaj, Feifei Pan*


#### Numerical Reasoning

- **Finqa: A dataset of numerical reasoning over financial data** `FinQANet` <ins>EMNLP</ins> 2021

   `FinQA`
   
    [[Paper](https://arxiv.org/abs/2109.00122)] [[Code](https://github.com/czyssrs/FinQA)] *Zhiyu Chen, Wenhu Chen, Charese Smiley, Sameena Shah, Iana Borova, Dylan Langdon, Reema Moussa, Matt Beane, Ting-Hao Huang, Bryan Routledge, William Yang Wang*

- **MultiHiertt: Numerical Reasoning over Multi Hierarchical Tabular and Textual Data** `MT2Net` <ins>ACL</ins> 2022

   `Multihiertt`
    
    [[Paper](https://aclanthology.org/2022.acl-long.454)] [[Code](https://github.com/psunlpgroup/MultiHiertt)]*Yilun Zhao, Yunxiang Li, Chenying Li, Rui Zhang*

- **APOLLO: An Optimized Training Approach for Long-form Numerical Reasoning** `APOLLO` <ins>Arxiv</ins> 2023

   `FinQA, ConvFinQA`

    [[Paper](https://arxiv.org/abs/2212.07249)] *Jiashuo Sun, Hang Zhang, Chen Lin, Yeyun Gong, Jian Guo, Nan Duan*

- **Dyrren: A dynamic retriever-reranker-generator model for numerical reasoning over tabular and textual data** `Dyrren` <ins>AAAI</ins> 2023

   `FinQA`
      
    [[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/26543)]  *Xiao Li, Yin Zhu, Sichen Liu, Jiangzhou Ju, Yuzhong Qu, Gong Cheng*

- **Hypothetical Training for Robust Machine Reading Comprehension of Tabular Context** `MT2Net` <ins>ACL-Findings</ins> 2023

   `TAT-QA, TAT-HQA`
       
    [[Paper](https://aclanthology.org/2023.findings-acl.79/)] *Moxin Li, Wenjie Wang, Fuli Feng, Hanwang Zhang, Qifan Wang, Tat-Seng Chua*

- **NAPG: Non-Autoregressive Program Generation for Hybrid Tabular-Textual Question Answering**  `NAPG` <ins>Arxiv</ins> 2023

   `Multihiertt`

    [[Paper](https://arxiv.org/abs/2211.03462)] *Tengxun Zhang, Hongfei Xu, Josef van Genabith, Deyi Xiong, Hongying Zan*


#### Open-Domain

- **Reasoning over hybrid chain for table-and-text open domain question answering** `CARP` <ins>IJCAI</ins> 2022

    `OTT-QA`

    [[Paper](https://www.ijcai.org/proceedings/2022/0629.pdf)] *Wanjun Zhong, Junjie Huang, Qian Liu, Ming Zhou, Jiahai Wang, Jian Yin, Nan Duan*

- **Mixed-modality Representation Learning and Pre-training for Joint Table-and-Text Retrieval in OpenQA**  `OTTeR` <ins>EMNLP-Findings</ins> 2022

    `OTT-QA`

    [[Paper](https://arxiv.org/abs/2210.05197)] *Junjie Huang, Wanjun Zhong, Qian Liu, Ming Gong, Daxin Jiang, Nan Duan*

- **Open-domain Question Answering via Chain of Reasoning over Heterogeneous Knowledge**  `CORE` <ins>EMNLP-Findings</ins> 2022

    `OTT-QA`

    [[Paper](https://arxiv.org/abs/2210.05197)] *Kaixin Ma, Hao Cheng, Xiaodong Liu, Eric Nyberg, Jianfeng Gao*

- **Chain-of-Skills: A Configurable Model for Open-domain Question Answering**  `CORE` <ins>ACL</ins> 2023

    `OTT-QA`

    [[Paper](https://arxiv.org/abs/2305.03130)] *Kaixin Ma, Hao Cheng, Yu Zhang, Xiaodong Liu, Eric Nyberg, Jianfeng Gao*

   

#### Multimodal Reasoning

- **MultiModalQA: complex question answering over text, tables and images** `ImplicitDecomp` <ins>ICLR</ins> 2021
   
    [[Paper](https://openreview.net/forum?id=ee6W5UgQLa)] [[Code](https://github.com/allenai/multimodalqa)]*Alon Talmor, Ori Yoran, Amnon Catav, Dan Lahav, Yizhong Wang, Akari Asai, Gabriel Ilharco, Hannaneh Hajishirzi, Jonathan Berant* 

- **MuRAG: Multimodal Retrieval-Augmented Generator for Open Question Answering over Images and Text**  `MuRAG` <ins>EMNLP</ins> 2022

   `MultimodalQA`

    [[Paper](https://aclanthology.org/2022.emnlp-main.375.pdf)] *Wenhu Chen, Hexiang Hu, Xi Chen, Pat Verga, William Cohen*

- **Turning Tables: Generating Examples from Semi-structured Tables for Endowing Language Models with Reasoning Skills** `SKURG` <ins>ACL</ins> 2022
   
   `MultimodalQA`

    [[Paper](https://aclanthology.org/2022.acl-long.416/)] *Ori Yoran, Alon Talmor, Jonathan Berant*




### Non-Retrieval Methods

- **TaCube: Pre-computing Data Cubes for Answering Numerical-Reasoning Questions over Tabular Data**  <ins>EMNLP</ins> 2022

    `TAT-QA, WikiTableQuestions`

    [[Paper](https://aclanthology.org/2022.emnlp-main.145.pdf)] *Fan Zhou, Mengkang Hu, Haoyu Dong, Zhoujun Cheng, Fan Cheng, Shi Han, Dongmei Zhang*

- **Answering Numerical Reasoning Questions in Table-Text Hybrid Contents with Graph-based Encoder and Tree-based Decoder**  <ins>COLING</ins> 2022

    `TAT-QA`

    [[Paper](https://arxiv.org/abs/2209.07692)] *Fangyu Lei, Shizhu He, Xiang Li, Jun Zhao, Kang Liu*

- **UniRPG: Unified Discrete Reasoning over Table and Text as Program Generation**  <ins>EMNLP</ins> 2022

    `TAT-QA`

    [[Paper](https://aclanthology.org/2022.emnlp-main.508/)] *Yongwei Zhou, Junwei Bao, Chaoqun Duan, Youzheng Wu, Xiaodong He, Tiejun Zhao*

- **Multi-View Graph Representation Learning for Answering Hybrid Numerical Reasoning Question**  <ins>Arxiv</ins> 2023

    `TAT-QA`

    [[Paper](https://arxiv.org/abs/2305.03458)] *Yifan Wei, Fangyu Lei, Yuanzhe Zhang, Jun Zhao, Kang Liu*


