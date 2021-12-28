# Paper Collection of Event

Recent conference papers exploring event on NLP (ACL, EMNLP, NAACL, COLING), AI (AAAI, IJCAI) and IR/DM (SIGIR, WWW, WSDM, KDD, CIKM).

## Overview

* [Event Reasoning](https://github.com/nudtzpan/Event-Papers#event-reasoning)
* [Event Causality Identification](https://github.com/nudtzpan/Event-Papers#event-causality-identification)
* [Event Temporal Relation Extraction](https://github.com/nudtzpan/Event-Papers#event-temporal-relation-extraction)

### Event Reasoning

* ESTER: A Machine Reading Comprehension Dataset for Reasoning about Event Semantic Relations. Rujun Han, I-Hung Hsu, Jiao Sun, Julia Baylon, Qiang Ning, Dan Roth, Nanyun Peng. EMNLP 2021 Full paper. [Code](https://github.com/PlusLabNLP/ESTER). <details>  <summary>Details</summary>  新数据集 包含5种事件间关系 </details>
* ExCAR: Event Graph Knowledge Enhanced Explainable Causal Reasoning. Li Du, Xiao Ding, Kai Xiong, Ting Liu, Bing Qin. ACL 2021 Full paper. [Code](https://github.com/sjcfr/xcar).
* Learning Event Graph Knowledge for Abductive Reasoning. Li Du, Xiao Ding, Ting Liu, Bing Qin. ACL 2021 Full paper. [Code](https://github.com/sjcfr/ege-RoBERTa).
* Modeling Event-Pair Relations in External Knowledge Graphs for Script Reasoning. Yucheng Zhou, Xiubo Geng, Tao Shen, Jian Pei, Wenqiang Zhang, Daxin Jiang. ACL Findings 2021 Full paper.

### Event Causality Identification

* LearnDA: Learnable Knowledge-Guided Data Augmentation for Event Causality Identification. Xinyu Zuo, Pengfei Cao, Yubo Chen, Kang Liu, Jun Zhao, Weihua Peng, Yuguang Chen. ACL 2021 Full paper.
* Knowledge-Enriched Event Causality Identification via Latent Structure Induction Networks. Pengfei Cao, Xinyu Zuo, Yubo Chen, Kang Liu, Jun Zhao, Yuguang Chen, Weihua Peng. ACL 2021 Full paper.
* Improving Event Causality Identification via Self-Supervised Representation Learning on External Causal Statement. Xinyu Zuo, Pengfei Cao, Yubo Chen, Kang Liu, Jun Zhao, Weihua Peng, Yuguang Chen. ACL Findings 2021 Full paper.
* Graph Convolutional Networks for Event Causality Identification with Rich Document-level Structures. Minh Tran Phu, Thien Huu Nguyen. NAACL 2021 Full paper.
* KnowDis: Knowledge Enhanced Data Augmentation for Event Causality Detection via Distant Supervision. Xinyu Zuo, Yubo Chen, Kang Liu, Jun Zhao. COLING 2020 Short paper.
* Knowledge Enhanced Event Causality Identification with Mention Masking Generalizations. Jian Liu, Yubo Chen, Jun Zhao. IJCAI 2020. [Code](https://github.com/jianliu-ml/EventCausalityIdentification).

### Event Temporal Relation Extraction

* Conditional Generation of Temporally-ordered Event Sequences. Shih-Ting Lin, Nathanael Chambers, Greg Durrett. ACL 2021 Full paper. [Code](https://github.com/jjasonn0717/TemporalBART). <details>  <summary>Details</summary>  Temporal Relation 采用自动化的方法从EventNarratives语料库中抽取时序事件，并采用BART模型进行编码和解码来做Temporal Event Ordering和Event Infilling的任务，其中使用Trick来对BART进行改进。 </details>

* Don't Let Discourse Confine Your Model: Sequence Perturbations for Improved Event Language Models. Mahnaz Koupaee, Greg Durrett, Nathanael Chambers, Niranjan Balasubramanian. ACL 2021 Short paper. [Code](https://github.com/StonyBrookNLP/elm-perturbations). <details>  <summary>Details</summary>  当前使用Event数据集进行训练时，Event之间的顺序直接采用的是Discourse中文本的顺序，但Event的顺序和Discourse的顺序可能并不相同。这就导致在训练时会引入偏差信息。作者提出采用事件打乱、事件Dropout以及事件Masking的数据增强方法来缓解错误的Event顺序对模型训练造成的不利影响。 </details>

* Embedding Time Differences in Context-sensitive Neural Networks for Learning Time to Event. Nazanin Dehghani, Hassan Hajipoor, Hadi Amiri. ACL 2021 Short paper. [Code](https://github.com/hajipoor/time2event). <details>  <summary>Details</summary>  给定事件E（时间戳，比如2017-08-24 18:00），给定Tweet A（时间戳：2017/08/24 11h，时间戳格式与事件E不同）和Tweet B（时间戳: 2017/08/24 08h）（Tweet A早于Tweet B），Tweet A是一个与事件E相关的Tweet，并且可能包含与事件E相关的时序信息（比如Tweet A里会说这周末发生事件E），目标就是预测Tweet B和事件E之间的前后顺序以及时间间隔。不是很理解，时间戳都有了，直接不就算出来了，可能是Tweet和事件的时间格式不一样？ </details>
* ECONET: Effective Continual Pretraining of Language Models for Event Temporal Reasoning. Rujun Han, Xiang Ren, Nanyun Peng. EMNLP 2021 Full paper. [Code](https://github.com/PlusLabNLP/ECONET). <details>  <summary>Details</summary>  新数据集 包含5种事件间关系 </details>
* Extracting Event Temporal Relations via Hyperbolic Geometry. Xingwei Tan, Gabriele Pergola, Yulan He. EMNLP 2021 Full paper. [Code](https://github.com/Xingwei-Warwick/hyper-event-TempRel). <details>  <summary>Details</summary>  新数据集 包含5种事件间关系 </details>
* Timeline Summarization based on Event Graph Compression via Time-Aware Optimal Transport. Manling Li, Tengfei Ma, Mo Yu, Lingfei Wu, Tian Gao, Heng Ji, Kathleen R. McKeown. EMNLP 2021 Full paper. [Code](https://github.com/limanling/event-graph-summarization). <details>  <summary>Details</summary>  新数据集 包含5种事件间关系 </details>
* Utilizing Relative Event Time to Enhance Event-Event Temporal Relation Extraction. Haoyang Wen, Heng Ji. EMNLP 2021 Short paper. [Code](https://github.com/wenhycs/EMNLP2021-Utilizing-Relative-Event-Time-to-Enhance-Event-Event-Temporal-Relation-Extraction). <details>  <summary>Details</summary>  新数据集 包含5种事件间关系 </details>
* Event Time Extraction and Propagation via Graph Attention Networks. Haoyang Wen, Yanru Qu, Heng Ji, Qiang Ning, Jiawei Han, Avi Sil, Hanghang Tong, Dan Roth. NAACL 2021 Full paper. [Code](https://github.com/wenhycs/NAACL2021-Event-Time-Extraction-and-Propagation-via-Graph-Attention-Networks). <details>  <summary>Details</summary>  新数据集 包含5种事件间关系 </details>
* EventPlus: A Temporal Event Understanding Pipeline. Mingyu Derek Ma, Jiao Sun, Mu Yang, Kung-Hsiang Huang, Nuan Wen, Shikhar Singh, Rujun Han, Nanyun Peng. NAACL 2021 Full paper. [Code](https://github.com/PlusLabNLP/EventPlus). <details>  <summary>Details</summary>  新数据集 包含5种事件间关系 </details>
* Temporal Reasoning on Implicit Events from Distant Supervision. Ben Zhou, Kyle Richardson, Qiang Ning, Tushar Khot, Ashish Sabharwal, Dan Roth. NAACL 2021 Full paper. [Code](https://github.com/allenai/tracie). <details>  <summary>Details</summary>  新数据集 包含5种事件间关系 </details>
* Time-Stamped Language Model: Teaching Language Models to Understand The Flow of Events. Hossein Rajaby Faghihi, Parisa Kordjamshidi. NAACL 2021 Full paper. [Code](https://github.com/HLR/TSLM). <details>  <summary>Details</summary>  新数据集 包含5种事件间关系 </details>
* Discourse-Level Event Temporal Ordering with Uncertainty-Guided Graph Completion. Jian Liu, Jinan Xu, Yufeng Chen, Yujie Zhang. IJCAI 2021. [Code](https://github.com/jianliu-ml/EventTemp). <details>  <summary>Details</summary>  新数据集 包含5种事件间关系 </details>
* Distinguishing Between Foreground and Background Events in News. Mohammed Aldawsari, Adrián Pérez, Deya Banisakher, Mark A. Finlayson. COLING 2020 Full paper. <details>  <summary>Details</summary>  新数据集 包含5种事件间关系 </details>
* Domain Knowledge Empowered Structured Neural Net for End-to-End Event Temporal Relation Extraction. Rujun Han, Yichao Zhou, Nanyun Peng. EMNLP 2020 Full paper. <details>  <summary>Details</summary>  新数据集 包含5种事件间关系 </details>
* Severing the Edge Between Before and After: Neural Architectures for Temporal Ordering of Events. Miguel Ballesteros, Rishita Anubhai, Shuai Wang, Nima Pourdamghani, Yogarshi Vyas, Jie Ma, Parminder Bhatia, Kathleen R. McKeown, Yaser Al-Onaizan. EMNLP 2020 Full paper. <details>  <summary>Details</summary>  新数据集 包含5种事件间关系 </details>
