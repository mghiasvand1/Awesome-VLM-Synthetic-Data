<div align="center">

<h1 id="survey-on-bridging-vlms-and-synthetic-data">[A Survey on Bridging VLMs and Synthetic Data](https://openreview.net/pdf?id=ThjDCZOljE)</h1>

</div>

<div align="center">

![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)

</div>

## <a id="abstract"></a>Abstract

Vision-language models (VLMs) have significantly advanced multimodal AI by learning joint representations of visual and textual data. However, their progress is hindered by challenges in acquiring high-quality, aligned datasets, including issues of cost, privacy, and scarcity. On the other hand, synthetic data, created through the use of generative AI—which can even include VLMs—offers a scalable and cost-effective solution to these challenges. This paper presents the first comprehensive survey on bridging VLMs and synthetic data, exploring both the role of synthetic data in VLMs and the role of VLMs in synthetic data. First, we provide a preliminary overview by briefly explaining the architecture of two basic VLMs and, after studying a large number of previous works, offer an extensive survey of the previously proposed methodologies and potential future directions in this area.

## <a id="citation"></a>Citation

If you find our paper useful for your work or research, please kindly cite it:
```
@article{mohammadkhani2025survey,
  title={A Survey on Bridging VLMs and Synthetic Data},
  author={Mohammadkhani, Mohammad Ghiasvand and Momtazi, Saeedeh and Beigy, Hamid},
  year={2025}
}
```

## Table of Content

- [Survey on Bridging VLMs and Synthetic data](#survey-on-bridging-vlms-and-synthetic-data)
  - [Abstract](#abstract)
  - [Reference](#reference)
  - [VLMs and Synthetic data](#vlms-synthetic-data)
    - [Instruction-Tuning & Alignment](#instruction-tuning--alignment)
    - [Evaluation](#evaluation)
    - [Multimodal Reasoning](#multimodal-reasoning)
    - [Retrieval-Augmented Tasks](#retrieval-augmented-tasks)
    - [Hallucination](#hallucination)
    - [Planning & Manipulation](#planning--manipulation)
    - [Regional Awareness & Visual Relations](#regional-awareness--visual-relations)
    - [Video-Centric Tasks](#video-centric-tasks)
    - [User Interface & Web Design](#user-interface--web-design)
    - [Grounding & Personalization](#grounding--personalization)
    - [Long-Context & Dialogue Handling](#long-context--dialogue-handling)
    - [Chart Understanding](#chart-understanding)
    - [3D Scene Comprehension](#3d-scene-comprehension)
    - [Image Captioning](#image-captioning)
    - [Multiculturalism & Multilingualism](#multiculturalism--multilingualism)
  - [Future Directions](#future-directions)
    - [Customized Data Synthesis](#customized-data-synthesis)
    - [In-Context Learning](#in-context-learning)
    - [Autonomous Driving](#autonomous-driving)
    - [Video-Level Analytics](#video-level-analytics)
    - [Dynamic Evaluation](#dynamic-evaluation)
    - [Low-Resource Settings](#low-resource-settings)
    - [Data Efficiency](#data-efficiency)

## <a id="vlms-synthetic-data"></a>VLMs and Synthetic Data

This section includes the surveyed works—grouped based on the main task they addressed—in which one of the following criteria is met: <b>(i)</b> <i>it proposes a synthetic data generation process utilizing VLMs and uses the data for an AI model</i>, or <b>(ii)</b> <i>it generates synthetic data without VLM involvement by using other generative AI models, such as LLMs or diffusion models, but later employs it for VLMs</i>. The first criterion addresses the role of VLMs in synthetic data and that of synthetic data (via VLMs) in VLMs, while the second considers the role of synthetic data (via non-VLM generative AI models) in VLMs—together examining both the role of VLMs in synthetic data and vice versa.

### <a id="instruction-tuning--alignment"></a>Instruction-Tuning & Alignment
- **Textbind: Multi-turn interleaved multimodal instruction-following in the wild** | *Huayang Li, Siheng Li, Deng Cai, Longyue Wang, Lemao Liu, Taro Watanabe, Yujiu Yang, and Shuming Shi* | ArXiv (2023) | [*paper*](https://arxiv.org/pdf/2309.08637)
- **Visual instruction tuning** | *Haotian Liu, Chunyuan Li, Qingyang Wu, and Yong Jae Lee* | NeurIPS (2023) | [*paper*](https://proceedings.neurips.cc/paper_files/paper/2023/file/6dcf277ea32ce3288914faf369fe6de0-Paper-Conference.pdf)
- **Llavar: Enhanced visual instruction tuning for text-rich image understanding** | *Yanzhe Zhang, Ruiyi Zhang, Jiuxiang Gu, Yufan Zhou, Nedim Lipka, Diyi Yang, and Tong Sun* | ArXiv (2023) | [*paper*](https://arxiv.org/pdf/2306.17107)
- **To see is to believe: Prompting gpt-4v for better visual instruction tuning** | *Junke Wang, Lingchen Meng, Zejia Weng, Bo He, Zuxuan Wu, and Yu-Gang Jiang* | ArXiv (2023) | [*paper*](https://arxiv.org/pdf/2311.07574)
- **Llava-med: Training a large language-and-vision assistant for biomedicine in one day** | *Chunyuan Li, Cliff Wong, Sheng Zhang, Naoto Usuyama, Haotian Liu, Jianwei Yang, Tristan Naumann, Hoifung Poon, and Jianfeng Gao* | NeurIPS (2023) | [*paper*](https://proceedings.neurips.cc/paper_files/paper/2023/file/5abcdf8ecdcacba028c6662789194572-Paper-Datasets_and_Benchmarks.pdf)
- **Enhancing large vision language models with self-training on image comprehension** | *Yihe Deng, Pan Lu, Fan Yin, Ziniu Hu, Sheng Shen, Quanquan Gu, James Y Zou, Kai-Wei Chang, and Wei Wang* | NeurIPS (2024) | [*paper*](https://proceedings.neurips.cc/paper_files/paper/2024/file/ed45d6a03de84cc650cae0655f699356-Paper-Conference.pdf)
- **VLFeedback: A Large-Scale AI Feedback Dataset for Large Vision-Language Models Alignment** | *Lei Li, Zhihui Xie, Mukai Li, Shunian Chen, Peiyi Wang, Liang Chen, Yazheng Yang, Benyou Wang, Lingpeng Kong, and Qi Liu* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2410.09421)
- **Drawing the Line: Enhancing Trustworthiness of MLLMs Through the Power of Refusal** | *Yuhao Wang, Zhiyuan Zhu, Heyang Liu, Yusheng Liao, Hongcheng Liu, Yanfeng Wang, and Yu Wang* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2412.11196)
- **Multimodal self-instruct: Synthetic abstract image and visual reasoning instruction using language model** | *Wenqi Zhang, Zhenglin Cheng, Yuanyu He, Mengna Wang, Yongliang Shen, Zeqi Tan, Guiyang Hou, Mingqian He, Yanna Ma, Weiming Lu, and Others* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2407.07053?)
- **Allava: Harnessing gpt4v-synthesized data for lite vision-language models** | *Guiming Hardy Chen, Shunian Chen, Ruifei Zhang, Junying Chen, Xiangbo Wu, Zhiyi Zhang, Zhihong Chen, Jianquan Li, Xiang Wan, and Benyou Wang* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2402.11684)
- **Agri-LLaVA: Knowledge-Infused Large Multimodal Assistant on Agricultural Pests and Diseases** | *Liqiong Wang, Teng Jin, Jinyu Yang, Ales Leonardis, Fangyi Wang, and Feng Zheng* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2412.02158)
- **MM-Instruct: Generated Visual Instructions for Large Multimodal Model Alignment** | *Jihao Liu, Xin Huang, Jinliang Zheng, Boxiao Liu, Jia Wang, Osamu Yoshie, Yu Liu, and Hongsheng Li* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2406.19736)
- **Vigc: Visual instruction generation and correction** | *Bin Wang, Fan Wu, Xiao Han, Jiahui Peng, Huaping Zhong, Pan Zhang, Xiaoyi Dong, Weijia Li, Wei Li, Jiaqi Wang, and Others* | AAAI (2024) | [*paper*](https://ojs.aaai.org/index.php/AAAI/article/view/28338/28664)
- **C3L: Content Correlated Vision-Language Instruction Tuning Data Generation via Contrastive Learning** | *Ji Ma, Wei Suo, Peng Wang, and Yanning Zhang* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2405.12752)
- **GENIXER: Empowering Multimodal Large Language Model as a Powerful Data Generator** | *Henry Hengyuan Zhao, Pan Zhou, and Mike Zheng Shou* | ECCV (2024) | [*paper*](https://arxiv.org/pdf/2312.06731)
- **Vision-flan: Scaling human-labeled tasks in visual instruction tuning** | *Zhiyang Xu, Chao Feng, Rulin Shao, Trevor Ashby, Ying Shen, Di Jin, Yu Cheng, Qifan Wang, and Lifu Huang* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2402.11690)
- **STLLaVA-Med: Self-Training Large Language and Vision Assistant for Medical Question-Answering** | *Guohao Sun, Can Qin, Huazhu Fu, Linwei Wang, and Zhiqiang Tao* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2406.19973?)
- **Biomedical visual instruction tuning with clinician preference alignment** | *Hejie Cui, Lingjun Mao, Xin Liang, Jieyu Zhang, Hui Ren, Quanzheng Li, Xiang Li, and Carl Yang* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2406.13173)
- **From Captions to Rewards (CAREVL): Leveraging Large Language Model Experts for Enhanced Reward Modeling in Large Vision-Language Models** | *Muzhi Dai, Jiashuo Sun, Zhiyuan Zhao, Shixuan Liu, Rui Li, Junyu Gao, and Xuelong Li* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2503.06260)
- **Omnialign-v: Towards enhanced alignment of mllms with human preference** | *Xiangyu Zhao, Shengyuan Ding, Zicheng Zhang, Haian Huang, Maosong Cao, Weiyun Wang, Jiaqi Wang, Xinyu Fang, Wenhai Wang, Guangtao Zhai, and Others* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2502.18411)
- **Unicorn: Text-Only Data Synthesis for Vision Language Model Training** | *Xiaomin Yu, Pengxiang Ding, Wenjie Zhang, Siteng Huang, Songyang Gao, Chengwei Qin, Kejian Wu, Zhaoxin Fan, Ziyue Qiao, and Donglin Wang* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2503.22655?)
- **EndoChat: Grounded Multimodal Large Language Model for Endoscopic Surgery** | *Guankun Wang, Long Bai, Junyi Wang, Kun Yuan, Zhen Li, Tianxu Jiang, Xiting He, Jinlin Wu, Zhen Chen, Zhen Lei, and Others* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2501.11347)
- **AnyPrefer: An Automatic Framework for Preference Data Synthesis** | *Yiyang Zhou, Zhaoyang Wang, Tianle Wang, Shangyu Xing, Peng Xia, Bo Li, Kaiyuan Zheng, Zijian Zhang, Zhaorun Chen, Wenhao Zheng, and Others* | ICLR (2025) | [*paper*](https://openreview.net/pdf?id=WpZyPk79Fu)
- **Scaling Text-Rich Image Understanding via Code-Guided Synthetic Multimodal Data Generation** | *Yue Yang, Ajay Patel, Matt Deitke, Tanmay Gupta, Luca Weihs, Andrew Head, Mark Yatskar, Chris Callison-Burch, Ranjay Krishna, Aniruddha Kembhavi, and Others* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2502.14846?)

### <a id="evaluation"></a>Evaluation
- **Large language models as automated aligners for benchmarking vision-language models** | *Yuanfeng Ji, Chongjian Ge, Weikai Kong, Enze Xie, Zhengying Liu, Zhengguo Li, and Ping Luo* | ArXiv (2023) | [*paper*](https://arxiv.org/pdf/2311.14580)
- **Autohallusion: Automatic generation of hallucination benchmarks for vision-language models** | *Xiyang Wu, Tianrui Guan, Dianqi Li, Shuaiyi Huang, Xiaoyu Liu, Xijun Wang, Ruiqi Xian, Abhinav Shrivastava, Furong Huang, Jordan Lee Boyd-Graber, and Others* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2406.10900)
- **MVP-Bench: Can Large Vision--Language Models Conduct Multi-level Visual Perception Like Humans?** | *Guanzhen Li, Yuxi Xie, and Min-Yen Kan* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2410.04345)
- **Vlbiasbench: A comprehensive benchmark for evaluating bias in large vision-language model** | *Sibo Wang, Xiangkui Cao, Jie Zhang, Zheng Yuan, Shiguang Shan, Xilin Chen, and Wen Gao* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2406.14194?)
- **Synthetic multimodal question generation** | *Ian Wu, Sravan Jayanthi, Vijay Viswanathan, Simon Rosenberg, Sina Pakazad, Tongshuang Wu, and Graham Neubig* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2407.02233)
- **VIVA: A Benchmark for Vision-Grounded Decision-Making with Human Values** | *Zhe Hu, Yixiao Ren, Jing Li, and Yu Yin* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2407.03000)
- **Mllm-as-a-judge: Assessing multimodal llm-as-a-judge with vision-language benchmark** | *Dongping Chen, Ruoxi Chen, Shilin Zhang, Yaochen Wang, Yinuo Liu, Huichi Zhou, Qihui Zhang, Yao Wan, Pan Zhou, and Lichao Sun* | ICML (2024) | [*paper*](https://openreview.net/pdf?id=dbFEFHAD79)
- **Prometheus-vision: Vision-language model as a judge for fine-grained evaluation** | *Seongyun Lee, Seungone Kim, Sue Park, Geewook Kim, and Minjoon Seo* | ACL (2024) | [*paper*](https://aclanthology.org/2024.findings-acl.672.pdf)
- **VLRewardBench: A Challenging Benchmark for Vision-Language Generative Reward Models** | *Lei Li, Yuancheng Wei, Zhihui Xie, Xuqing Yang, Yifan Song, Peiyi Wang, Chenxin An, Tianyu Liu, Sujian Li, Bill Yuchen Lin, and Others* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2411.17451)
- **Conme: Rethinking evaluation of compositional reasoning for modern vlms** | *Irene Huang, Wei Lin, Muhammad Jehanzeb Mirza, Jacob Hansen, Sivan Doveh, Victor Butoi, Roei Herzig, Assaf Arbelle, Hilde Kuehne, Trevor Darrell, and Others* | NeurIPS (2024) | [*paper*](https://proceedings.neurips.cc/paper_files/paper/2024/file/28aad3b3b315d86910d7f4ee2867dfa4-Paper-Datasets_and_Benchmarks_Track.pdf)
- **Less-to-more generalization: Unlocking more controllability by in-context generation** | *Shaojin Wu, Mengqi Huang, Wenxu Wu, Yufeng Cheng, Fei Ding, and Qian He* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2504.02160)
- **Does Your Vision-Language Model Get Lost in the Long Video Sampling Dilemma?** | *Tianyuan Qu, Longxiang Tang, Bohao Peng, Senqiao Yang, Bei Yu, and Jiaya Jia* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2503.12496?)
- **Structured Preference Optimization for Vision-Language Long-Horizon Task Planning** | *Xiwen Liang, Min Lin, Weiqi Ruan, Rongtao Xu, Yuecheng Liu, Jiaqi Chen, Bingqian Lin, Yuzheng Zhuang, and Xiaodan Liang* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2502.20742?)
- **When'YES'Meets' BUT': Can Large Models Comprehend Contradictory Humor Through Comparative Reasoning?** | *Tuo Liang, Zhe Hu, Jing Li, Hao Zhang, Yiren Lu, Yunlai Zhou, Yiran Qiao, Disheng Liu, Jeirui Peng, Jing Ma, and Others* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2503.23137)
- **DrawEduMath: Evaluating Vision Language Models with Expert-Annotated Students' Hand-Drawn Math Images** | *Sami Baral, Li Lucy, Ryan Knight, Alice Ng, Luca Soldaini, Neil T Heffernan, and Kyle Lo* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2501.14877)
- **KITAB-Bench: A Comprehensive Multi-Domain Benchmark for Arabic OCR and Document Understanding** | *Ahmed Heakl, Abdullah Sohail, Mukul Ranjan, Rania Hossam, Ghazi Ahmed, Mohamed El-Geish, Omar Maher, Zhiqiang Shen, Fahad Khan, and Salman Khan* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2502.14949)

### <a id="multimodal-reasoning"></a>Multimodal Reasoning
- **What makes for good visual instructions? synthesizing complex visual reasoning instructions for visual instruction tuning** | *Yifan Du, Hangyu Guo, Kun Zhou, Wayne Xin Zhao, Jinpeng Wang, Chuyuan Wang, Mingchen Cai, Ruihua Song, and Ji-Rong Wen* | ArXiv (2023) | [*paper*](https://arxiv.org/pdf/2311.01487)
- **Navgpt-2: Unleashing navigational reasoning capability for large vision-language models** | *Gengze Zhou, Yicong Hong, Zun Wang, Xin Eric Wang, and Qi Wu* | ECCV (2024) | [*paper*](https://arxiv.org/pdf/2407.12366)
- **Visual program distillation: Distilling tools and programmatic reasoning into vision-language models** | *Yushi Hu, Otilia Stretcu, Chun-Ta Lu, Krishnamurthy Viswanathan, Kenji Hata, Enming Luo, Ranjay Krishna, and Ariel Fuxman* | CVPR (2024) | [*paper*](http://openaccess.thecvf.com/content/CVPR2024/papers/Hu_Visual_Program_Distillation_Distilling_Tools_and_Programmatic_Reasoning_into_Vision-Language_CVPR_2024_paper.pdf)
- **R-cot: Reverse chain-of-thought problem generation for geometric reasoning in large multimodal models** | *Linger Deng, Yuliang Liu, Bohan Li, Dongliang Luo, Liang Wu, Chengquan Zhang, Pengyuan Lyu, Ziyang Zhang, Gang Zhang, Errui Ding, and Others* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2410.17885)
- **Math-llava: Bootstrapping mathematical reasoning for multimodal large language models** | *Wenhao Shi, Zhiqiang Hu, Yi Bin, Junhua Liu, Yang Yang, See-Kiong Ng, Lidong Bing, and Roy Ka-Wei Lee* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2406.17294)
- **Improve vision language model chain-of-thought reasoning** | *Ruohong Zhang, Bowen Zhang, Yanghao Li, Haotian Zhang, Zhiqing Sun, Zhe Gan, Yinfei Yang, Ruoming Pang, and Yiming Yang* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2410.16198?)
- **From the least to the most: Building a plug-and-play visual reasoner via data synthesis** | *Chuanqi Cheng, Jian Guan, Wei Wu, and Rui Yan* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2406.19934?)
- **URSA: Understanding and Verifying Chain-of-thought Reasoning in Multimodal Mathematics** | *Ruilin Luo, Zhuofan Zheng, Yifan Wang, Yiyao Yu, Xinzhe Ni, Zicheng Lin, Jin Zeng, and Yujiu Yang* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2501.04686)
- **Mm-verify: Enhancing multimodal reasoning with chain-of-thought verification** | *Linzhuang Sun, Hao Liang, Jingxuan Wei, Bihui Yu, Tianpeng Li, Fan Yang, Zenan Zhou, and Wentao Zhang* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2502.13383)
- **SMIR: Efficient Synthetic Data Pipeline To Improve Multi-Image Reasoning** | *Andrew Li, Rahul Thapa, Rahul Chalamala, Qingyang Wu, Kezhen Chen, and James Zou* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2501.03675)
- **TACO: Learning Multi-modal Models to Reason and Act with Synthetic Chains-of-Thought-and-Action** | *Zixian Ma, Jianguo Zhang, Zhiwei Liu, Jieyu Zhang, Juntao Tan, Manli Shu, Juan Carlos Niebles, Shelby Heinecke, Huan Wang, Caiming Xiong, and Others* | ICLR (2025) | [*paper*](https://openreview.net/pdf?id=8fty8ubFmm)
- **When Words Outperform Vision: VLMs Can Self-Improve Via Text-Only Training For Human-Centered Decision Making** | *Zhe Hu, Jing Li, and Yu Yin* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2503.16965?)
- **Enhancing Compositional Reasoning in Vision-Language Models with Synthetic Preference Data** | *Samarth Mishra, Kate Saenko, and Venkatesh Saligrama* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2504.04740)
- **MindGYM: Enhancing Vision-Language Models via Synthetic Self-Challenging Questions** | *Zhe Xu, Daoyuan Chen, Zhenqing Ling, Yaliang Li, and Ying Shen* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2503.09499)
- **MMR: A Large-scale Benchmark Dataset for Multi-target and Multi-granularity Reasoning Segmentation** | *Donggon Jang, Yucheol Cho, Suin Lee, Taehyeon Kim, and Dae-Shik Kim* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2503.13881?)

### <a id="retrieval-augmented-tasks"></a>Retrieval-Augmented Tasks
- **Visual chain of thought: bridging logical gaps with multimodal infillings** | *Daniel Rose, Vaishnavi Himakunthala, Andy Ouyang, Ryan He, Alex Mei, Yujie Lu, Michael Saxon, Chinmay Sonar, Diba Mirza, and William Yang Wang* | ArXiv (2023) | [*paper*](https://arxiv.org/pdf/2305.02317)
- **MegaPairs: Massive Data Synthesis For Universal Multimodal Retrieval** | *Junjie Zhou, Zheng Liu, Ze Liu, Shitao Xiao, Yueze Wang, Bo Zhao, Chen Jason Zhang, Defu Lian, and Yongping Xiong* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2412.14475)
- **Visrag: Vision-based retrieval-augmented generation on multi-modality documents** | *Shi Yu, Chaoyue Tang, Bokai Xu, Junbo Cui, Junhao Ran, Yukun Yan, Zhenghao Liu, Shuo Wang, Xu Han, Zhiyuan Liu, and Others* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2410.10594)
- **Compositional Image Retrieval via Instruction-Aware Contrastive Learning** | *Wenliang Zhong, Weizhi An, Feng Jiang, Hehuan Ma, Yuzhi Guo, and Junzhou Huang* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2412.05756)
- **VISA: Retrieval Augmented Generation with Visual Source Attribution** | *Xueguang Ma, Shengyao Zhuang, Bevan Koopman, Guido Zuccon, Wenhu Chen, and Jimmy Lin* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2412.05756)
- **SK-VQA: Synthetic Knowledge Generation at Scale for Training Context-Augmented Multimodal LLMs** | *Xin Su, Man Luo, Kris W Pan, Tien Pei Chou, Vasudev Lal, and Phillip Howard* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2406.19593)
- **Vision-language models do not understand negation** | *Kumail Alhamoud, Shaden Alshammari, Yonglong Tian, Guohao Li, Philip Torr, Yoon Kim, and Marzyeh Ghassemi* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2501.09425)
- **ImageRef-VL: Enabling Contextual Image Referencing in Vision-Language Models** | *Jingwei Yi, Junhao Yin, Ju Xu, Peng Bao, Yongliang Wang, Wei Fan, and Hao Wang* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2501.12418)
- **good4cir: Generating Detailed Synthetic Captions for Composed Image Retrieval** | *Pranavi Kolouju, Eric Xing, Robert Pless, Nathan Jacobs, and Abby Stylianou* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2503.17871)

### <a id="hallucination"></a>Hallucination
- **Ciem: Contrastive instruction evaluation method for better instruction tuning** | *Hongyu Hu, Jiyuan Zhang, Minyi Zhao, and Zhenbang Sun* | ArXiv (2023) | [*paper*](https://arxiv.org/pdf/2309.02301)
- **HallE-Control: controlling object hallucination in large multimodal models** | *Bohan Zhai, Shijia Yang, Chenfeng Xu, Sheng Shen, Kurt Keutzer, Chunyuan Li, and Manling Li* | ArXiv (2023) | [*paper*](https://arxiv.org/pdf/2310.01779)
- **Mitigating open-vocabulary caption hallucinations** | *Assaf Ben-Kish, Moran Yanuka, Morris Alper, Raja Giryes, and Hadar Averbuch-Elor* | ArXiv (2023) | [*paper*](https://arxiv.org/pdf/2312.03631)
- **Aligning large multi-modal model with robust instruction tuning** | *Fuxiao Liu, Kevin Lin, Linjie Li, Jianfeng Wang, Yaser Yacoob, and Lijuan Wang* | ICLR (2023) | [*paper*](https://arxiv.org/pdf/2306.14565v4)
- **VGA: Vision GUI Assistant-Minimizing Hallucinations through Image-Centric Fine-Tuning** | *Meng Ziyang, Yu Dai, Zezheng Gong, Shaoxiong Guo, Minglong Tang, and Tongquan Wei* | EMNLP (2024) | [*paper*](https://aclanthology.org/2024.findings-emnlp.68.pdf)
- **V-dpo: Mitigating hallucination in large vision language models via vision-guided direct preference optimization** | *Yuxi Xie, Guanzhen Li, Xiao Xu, and Min-Yen Kan* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2411.02712)
- **Tldr: Token-level detective reward model for large vision language models** | *Deqing Fu, Tong Xiao, Rui Wang, Wang Zhu, Pengchuan Zhang, Guan Pang, Robin Jia, and Lawrence Chen* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2410.04734)
- **LongHalQA: Long-Context Hallucination Evaluation for MultiModal Large Language Models** | *Han Qiu, Jiaxing Huang, Peng Gao, Qin Qi, Xiaoqin Zhang, Ling Shao, and Shijian Lu* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2410.09962)

### <a id="planning--manipulation"></a>Planning & Manipulation
- **Embodied task planning with large language models** | *Zhenyu Wu, Ziwei Wang, Xiuwei Xu, Jiwen Lu, and Haibin Yan* | ArXiv (2023) | [*paper*](https://arxiv.org/pdf/2307.01848)
- **Robotic control via embodied chain-of-thought reasoning** | *Michał Zawalski, William Chen, Karl Pertsch, Oier Mees, Chelsea Finn, and Sergey Levine* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2407.08693)
- **ReLEP: A Novel Framework for Real-world Long-horizon Embodied Planning** | *Siyuan Liu, Jiawei Du, Sicheng Xiang, Zibo Wang, and Dingsheng Luo* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2409.15658)
- **Manipulate-anything: Automating real-world robots using vision-language models** | *Jiafei Duan, Wentao Yuan, Wilbert Pumacay, Yi Ru Wang, Kiana Ehsani, Dieter Fox, and Ranjay Krishna* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2406.18915)
- **Cogcom: Train large vision-language models diving into details through chain of manipulations** | *Ji Qi, Ming Ding, Weihan Wang, Yushi Bai, Qingsong Lv, Wenyi Hong, Bin Xu, Lei Hou, Juanzi Li, Yuxiao Dong, and Others* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2402.04236)
- **Multi-modal Agent Tuning: Building a VLM-Driven Agent for Efficient Tool Usage** | *Zhi Gao, Bofei Zhang, Pengxiang Li, Xiaojian Ma, Tao Yuan, Yue Fan, Yuwei Wu, Yunde Jia, Song-Chun Zhu, and Qing Li* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2412.15606?)
- **HybridGen: VLM-Guided Hybrid Planning for Scalable Data Generation of Imitation Learning** | *Wensheng Wang, and Ning Tan* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2503.13171?)

### <a id="regional-awareness--visual-relations"></a>Regional Awareness & Visual Relations
- **Regiongpt: Towards region understanding vision language model** | *Qiushan Guo, Shalini De Mello, Hongxu Yin, Wonmin Byeon, Ka Chun Cheung, Yizhou Yu, Ping Luo, and Sifei Liu* | CVPR (2024) | [*paper*](https://openaccess.thecvf.com/content/CVPR2024/papers/Guo_RegionGPT_Towards_Region_Understanding_Vision_Language_Model_CVPR_2024_paper.pdf)
- **Relationvlm: Making large vision-language models understand visual relations** | *Zhipeng Huang, Zhizheng Zhang, Zheng-Jun Zha, Yan Lu, and Baining Guo* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2403.12801)
- **VisMin: Visual Minimal-Change Understanding** | *Rabiul Awal, Saba Ahmadi, Le Zhang, and Aishwarya Agrawal* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2407.16772)
- **Right this way: Can VLMs Guide Us to See More to Answer Questions?** | *Li Liu, Diji Yang, Sijia Zhong, Kalyana Suma Sree Tholeti, Lei Ding, Yi Zhang, and Leilani Gilpin* | NeurIPS (2024) | [*paper*](https://proceedings.neurips.cc/paper_files/paper/2024/file/efe4e50d492fedc0dfd2959f3320a974-Paper-Conference.pdf)
- **COCONut-PanCap: Joint Panoptic Segmentation and Grounded Captions for Fine-Grained Understanding and Generation** | *Xueqing Deng, Qihang Yu, Ali Athar, Chenglin Yang, Linjie Yang, Xiaojie Jin, Xiaohui Shen, and Liang-Chieh Chen* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2502.02589)
- **Pixel-Level Reasoning Segmentation via Multi-turn Conversations** | *Dexian Cai, Xiaocui Yang, Yongkang Liu, Daling Wang, Shi Feng, Yifei Zhang, and Soujanya Poria* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2502.09447)
- **Enhancing Vision-Language Compositional Understanding with Multimodal Synthetic Data** | *Haoxin Li, and Boyang Li* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2503.01167)

### <a id="video-centric-tasks"></a>Video-Centric Tasks
- **Inst-IT: Boosting Multimodal Instance Understanding via Explicit Visual Prompt Instruction Tuning** | *Wujian Peng, Lingchen Meng, Yitong Chen, Yiweng Xie, Yang Liu, Tao Gui, Hang Xu, Xipeng Qiu, Zuxuan Wu, and Yu-Gang Jiang* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2412.03565)
- **Video-xl: Extra-long vision language model for hour-scale video understanding** | *Yan Shu, Zheng Liu, Peitian Zhang, Minghao Qin, Junjie Zhou, Zhengyang Liang, Tiejun Huang, and Bo Zhao* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2409.14485)
- **Cogvlm2: Visual language models for image and video understanding** | *Wenyi Hong, Weihan Wang, Ming Ding, Wenmeng Yu, Qingsong Lv, Yan Wang, Yean Cheng, Shiyu Huang, Junhui Ji, Zhao Xue, and Others* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2408.16500)
- **Video instruction tuning with synthetic data** | *Yuanhan Zhang, Jinming Wu, Wei Li, Bo Li, Zejun Ma, Ziwei Liu, and Chunyuan Li* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2410.02713)
- **Cogvideox: Text-to-video diffusion models with an expert transformer** | *Zhuoyi Yang, Jiayan Teng, Wendi Zheng, Ming Ding, Shiyu Huang, Jiazheng Xu, Yuanming Yang, Wenyi Hong, Xiaohan Zhang, Guanyu Feng, and Others* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2408.06072)
- **VITED: Video Temporal Evidence Distillation** | *Yujie Lu, Yale Song, William Wang, Lorenzo Torresani, and Tushar Nagarajan* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2503.12855)

### <a id="user-interface--web-design"></a>User Interface & Web Design
- **Dreamstruct: Understanding slides and user interfaces via synthetic data generation** | *Yi-Hao Peng, Faria Huq, Yue Jiang, Jason Wu, Xin Yue Li, Jeffrey P Bigham, and Amy Pavel* | ECCV (2024) | [*paper*](https://arxiv.org/pdf/2410.00201)
- **Ferret-ui 2: Mastering universal user interface understanding across platforms** | *Zhangheng Li, Keen You, Haotian Zhang, Di Feng, Harsh Agrawal, Xiujun Li, Mohana Prasad Sathya Moorthy, Jeff Nichols, Yinfei Yang, and Zhe Gan* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2410.18967)
- **Screenai: A vision-language model for ui and infographics understanding** | *Gilles Baechler, Srinivas Sunkara, Maria Wang, Fedir Zubach, Hassan Mansoor, Vincent Etter, Victor Carbune, Jason Lin, Jindong Che, and Abhanshu Sharma* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2402.04615)
- **Unlocking the conversion of web screenshots into html code with the websight dataset** | *Hugo Laurençon,  Léo Tronchon, and Victor Sanh* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2403.09029)
- **Iluvui: Instruction-tuned language-vision modeling of uis from machine conversations** | *Yue Jiang, Eldon Schoop, Amanda Swearngin, and Jeffrey Nichols* | IUI (2025) | [*paper*](https://dl.acm.org/doi/pdf/10.1145/3708359.3712129)
- **Advancing vision-language models in front-end development via data synthesis** | *Tong Ge, Yashu Liu, Jieping Ye, Tianyi Li, and Chao Wang* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2503.01619)

### <a id="grounding--personalization"></a>Grounding & Personalization
- **Learning to Ground VLMs without Forgetting** | *Aritra Bhowmik, Mohammad Mahdi Derakhshani, Dennis Koelma, Martin R Oswald, Yuki M Asano, and Cees GM Snoek* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2410.10491)
- **Learning from Synthetic Data for Visual Grounding** | *Ruozhen He, Ziyan Yang, Paola Cascante-Bonilla, Alexander C Berg, and Vicente Ordonez* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2403.13804)
- **Personalized Large Vision-Language Models** | *Chau Pham, Hoang Phan, David Doermann, and Yunjie Tian* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2412.17610)
- **Towards Visual Text Grounding of Multimodal Large Language Model** | *Ming Li, Ruiyi Zhang, Jian Chen, Jiuxiang Gu, Yufan Zhou, Franck Dernoncourt, Wanrong Zhu, Tianyi Zhou, and Tong Sun* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2504.04974)
- **Concept-as-Tree: Synthetic Data is All You Need for VLM Personalization** | *Ruichuan An, Kai Zeng, Ming Lu, Sihan Yang, Renrui Zhang, Huitong Ji, Qizhe Zhang, Yulin Luo, Hao Liang, and Wentao Zhang* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2503.12999)

### <a id="long-context--dialogue-handling"></a>Long-Context & Dialogue Handling
- **Going beyond Imagination! Enhancing Multi-modal Dialogue Agents with Synthetic Visual Descriptions** | *Haolan Zhan, Sameen Maruf, Ingrid Zukerman, and Gholamreza Haffari* | SIGDial (2024) | [*paper*](https://aclanthology.org/2024.sigdial-1.36.pdf)
- **Fire: A dataset for feedback integration and refinement evaluation of multimodal models** | *Pengxiang Li, Zhi Gao, Bofei Zhang, Tao Yuan, Yuwei Wu, Mehrtash Harandi, Yunde Jia, Song-Chun Zhu, and Qing Li* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2407.11522)
- **Enhanced Visual Instruction Tuning with Synthesized Image-Dialogue Data** | *Yanda Li, Chi Zhang, Gang Yu, Wanqi Yang, Zhibin Wang, Bin Fu, Guosheng Lin, Chunhua Shen, Ling Chen, and Yunchao Wei* | ACL (2024) | [*paper*](https://aclanthology.org/2024.findings-acl.864.pdf)
- **Insight-v: Exploring long-chain visual reasoning with multimodal large language models** | *Yuhao Dong, Zuyan Liu, Hai-Long Sun, Jingkang Yang, Winston Hu, Yongming Rao, and Ziwei Liu* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2411.14432)
- **Longwriter-v: Enabling ultra-long and high-fidelity generation in vision-language models** | *Shangqing Tu, Yucheng Wang, Daniel Zhang-Li, Yushi Bai, Jifan Yu, Yuhao Wu, Lei Hou, Huiqin Liu, Zhiyuan Liu, Bin Xu, and Others* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2502.14834)

### <a id="chart-understanding"></a>Chart Understanding
- **Chartllama: A multimodal llm for chart understanding and generation** | *Yucheng Han, Chi Zhang, Xin Chen, Xu Yang, Zhibin Wang, Gang Yu, Bin Fu, and Hanwang Zhang* | ArXiv (2023) | [*paper*](https://arxiv.org/pdf/2311.16483)
- **Evochart: A benchmark and a self-training approach towards real-world chart understanding** | *Muye Huang, Han Lai, Xinyu Zhang, Wenjun Wu, Jie Ma, Lingling Zhang, and Jun Liu* | AAAI (2025) | [*paper*](https://ojs.aaai.org/index.php/AAAI/article/download/32383/34538)
- **RefChartQA: Grounding Visual Answer on Chart Images through Instruction Tuning** | *Alexander Vogel, Omar Moured, Yufan Chen, Jiaming Zhang, and Rainer Stiefelhagen* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2503.23131)
- **ChartCoder: Advancing Multimodal Large Language Model for Chart-to-Code Generation** | *Xuanle Zhao, Xianzhen Luo, Qi Shi, Chi Chen, Shuo Wang, Wanxiang Che, Zhiyuan Liu, and Maosong Sun* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2501.06598)
- **Chain of Functions: A Programmatic Pipeline for Fine-Grained Chart Reasoning Data** | *Zijian Li, Jingjing Fu, Lei Song, Jiang Bian, Jun Zhang, and Rui Wang* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2503.16260?)

### <a id="3d-scene-comprehension"></a>3D Scene Comprehension
- **ChatGarment: Garment Estimation, Generation and Editing via Large Language Models** | *Siyuan Bian, Chenghao Xu, Yuliang Xiu, Artur Grigorev, Zhen Liu, Cewu Lu, Michael J Black, and Yao Feng* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2412.17811?)
- **Multimodal 3D Reasoning Segmentation with Complex Scenes** | *Xueying Jiang, Lewei Lu, Ling Shao, and Shijian Lu* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2411.13927)
- **Spatialvlm: Endowing vision-language models with spatial reasoning capabilities** | *Boyuan Chen, Zhuo Xu, Sean Kirmani, Brain Ichter, Dorsa Sadigh, Leonidas Guibas, and Fei Xia* | CVPR (2024) | [*paper*](https://openaccess.thecvf.com/content/CVPR2024/papers/Chen_SpatialVLM_Endowing_Vision-Language_Models_with_Spatial_Reasoning_Capabilities_CVPR_2024_paper.pdf)
- **Pisa: A self-augmented data engine and training strategy for 3d understanding with large models** | *Zilu Guo, Hongbin Lin, Zhihao Yuan, Chaoda Zheng, Pengshuo Qiu, Dongzhi Jiang, Renrui Zhang, Chun-Mei Feng, and Zhen Li* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2503.10529)
- **3UR-LLM: An End-to-End Multimodal Large Language Model for 3D Scene Understanding** | *Haomiao Xiong, Yunzhi Zhuge, Jiawen Zhu, Lu Zhang, and Huchuan Lu* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2501.07819)

### <a id="image-captioning"></a>Image Captioning
- **BLIP3-KALE: Knowledge Augmented Large-Scale Dense Captions** | *Anas Awadalla, Le Xue, Manli Shu, An Yan, Jun Wang, Senthil Purushwalkam, Sheng Shen, Hannah Lee, Oscar Lo, Jae Sung Park, and Others* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2411.07461)
- **VILA 2: VILA Augmented VILA** | *Yunhao Fang, Ligeng Zhu, Yao Lu, Yan Wang, Pavlo Molchanov, Jan Kautz, Jang Hyun Cho, Marco Pavone, Song Han, and Hongxu Yin* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2407.17453)
- **Benchmarking and improving detail image caption** | *Hongyuan Dong, Jiawen Li, Bohong Wu, Jiacong Wang, Yuan Zhang, and Haoyuan Guo* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2405.19092)
- **Synthvlm: High-efficiency and high-quality synthetic data for vision language models** | *Zheng Liu, Hao Liang, Xijie Huang, Wentao Xiong, Qinhan Yu, Linzhuang Sun, Chong Chen, Conghui He, Bin Cui, and Wentao Zhang* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2407.20756)

### <a id="multiculturalism--multilingualism"></a>Multiculturalism & Multilingualism
- **X-llava: Optimizing bilingual large vision-language alignment** | *Dongjae Shin, HyeonSeok Lim, Inho Won, Changsu Choi, Minjun Kim, Seungwoo Song, Hangyeol Yoo, Sangmin Kim, and Kyungtae Lim* | ArXiv (2024) | [*paper*](https://arxiv.org/pdf/2403.11399)
- **CultureVLM: Characterizing and Improving Cultural Understanding of Vision-Language Models for over 100 Countries** | *Shudong Liu, Yiqiao Jin, Cheng Li, Derek F Wong, Qingsong Wen, Lichao Sun, Haipeng Chen, Xing Xie, and Jindong Wang* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2501.01282)
- **When Tom Eats Kimchi: Evaluating Cultural Bias of Multimodal Large Language Models in Cultural Mixture Contexts** | *Jun Seong Kim, Kyaw Ye Thu, Javad Ismayilzada, Junyeong Park, Eunsu Kim, Huzama Ahmad, Na Min An, James Thorne, and Alice Oh* | ArXiv (2025) | [*paper*](https://arxiv.org/pdf/2503.16826?)

## <a id="future-directions"></a>Future Directions

While extensive efforts have been made to bridge the contents of VLMs and synthetic data, several unexplored paths still offer great promise, and we outline a few ones that could spark future research.

### <a id="customized-data-synthesis"></a>Customized Data Synthesis
Data for or by VLMs is often generated with fixed goals and limited customization. Training an open-source model for multimodal data or task generation with customizable properties would be highly valuable.

### <a id="in-context-learning"></a>In-Context Learning
As a training-free approach, it offers a valuable way to capture patterns via in-context demonstrations. Future work may focus on generating data as effective in context examples and refining task prompts to ensure the examples instill better task understanding.

### <a id="autonomous-driving"></a>Autonomous Driving
These systems need real-time understanding of dynamic environments, making them well-suited for robust VLMs. Due to the difficulty of collecting quality data, future research may focus on generating synthetic scenarios or using them to tune or evaluate VLMs.

### <a id="video-level-analytics"></a>Video-Level Analytics
Many applications require reporting specific actions in videos. These can be addressed by methods that track various visual elements across frames to analyze their behavior and actions throughout the video.

### <a id="dynamic-evaluation"></a>Dynamic Evaluation
Similar to approaches for LLMs, a multi-turn dynamic evaluation setup for VLMs can help avoid issues like contamination while simultaneously improving the model through synthetic data generated within the evaluation process.

### <a id="low-resource-settings"></a>Low-Resource Settings
VLMs mainly advance in high-resource domains, while many regions lack labeled multimodal data. Synthetic pipelines can bridge this gap by generating data in underrepresented languages, cultures, and applications for further processing.

### <a id="data-efficiency"></a>Data Efficiency
With growing model sizes, maximizing data efficiency is crucial. While synthetic data is often generated at scale, applying quality and diversity measures can reduce data volume for better cost and resource use.
