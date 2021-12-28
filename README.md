# Paper Collection of Event

Recent conference papers exploring event on NLP (ACL, EMNLP, NAACL, COLING), AI (AAAI, IJCAI) and IR/DM (SIGIR, WWW, WSDM, KDD, CIKM).

## Overview

* [Event Reasoning](https://github.com/nudtzpan/Event-Papers#event-reasoning)
* [Event Causality Identification](https://github.com/nudtzpan/Event-Papers#event-causality-identification)
* [Event Temporal Relation Extraction](https://github.com/nudtzpan/Event-Papers#event-temporal-relation-extraction)

### Event Reasoning

* ESTER: A Machine Reading Comprehension Dataset for Reasoning about Event Semantic Relations. Rujun Han, I-Hung Hsu, Jiao Sun, Julia Baylon, Qiang Ning, Dan Roth, Nanyun Peng. EMNLP 2021 Full paper. [Code](https://github.com/PlusLabNLP/ESTER). <details>  <summary>Details</summary>  新数据集 包含5种事件间关系 </details>
* From Discourse to Narrative: Knowledge Projection for Event Relation Extraction. Jialong Tang, Hongyu Lin, Meng Liao, Yaojie Lu, Xianpei Han, Le Sun, Weijian Xie, Jin Xu. ACL 2021 Full paper. [Code](https://github.com/TangJiaLong/Knowledge-Projection-for-ERE). <details>  <summary>Details</summary>  把Discourse里的Knowledge Project到Event Relation Extraction中（分为token-level，semantic-level以及label-level），辅助学习BERT-based Token Encoder，VAE-based Semantic Encoder以及Coarse Category Encoder。基于ASER数据集进行处理得到IERE数据集，没说Relation种类有多少。 </details>
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

* ECONET: Effective Continual Pretraining of Language Models for Event Temporal Reasoning. Rujun Han, Xiang Ren, Nanyun Peng. EMNLP 2021 Full paper. [Code](https://github.com/PlusLabNLP/ECONET). <details>  <summary>Details</summary>  预训练模型没有将事件以及事件间时序顺序考虑进来，因此本文针对event relation extraction (ERE)和machine reading comprehension (MRC)，提出targeted masking来mask event trigger words和temporal indicators。并且在Temporal Generator和Event Generator的基础上加入Contrastive loss来对模型进行训练（不是很理解，已经有了Temporal loss和Event loss，为什么还需要Contrastive loss?）另外本文采用Continual Pretraining的训练方式，没理解啥意思。 </details>

* Extracting Event Temporal Relations via Hyperbolic Geometry. Xingwei Tan, Gabriele Pergola, Yulan He. EMNLP 2021 Full paper. [Code](https://github.com/Xingwei-Warwick/hyper-event-TempRel). <details>  <summary>Details</summary>  作者认为传统的欧几里得空间无法捕获丰富的非对称关系，比如（事件A导致事件B，但事件B并不一定导致事件A），因此提出利用Hyperbolic Geometry 双曲几何来embed events。具体细节没仔细看。 </details>

* Timeline Summarization based on Event Graph Compression via Time-Aware Optimal Transport. Manling Li, Tengfei Ma, Mo Yu, Lingfei Wu, Tian Gao, Heng Ji, Kathleen R. McKeown. EMNLP 2021 Full paper. [Code](https://github.com/limanling/event-graph-summarization). <details>  <summary>Details</summary>  给定一系列包含事件的文本，从文本中总结出事件的时间线。以往方法首先确定事件的关键日期，然后为每一天分别进行总结，这样的方法忽略了时间内部Argument之间的联系以及事件与事件之间的联系，因此作者提出将这一系列包含事件的文本构造成Event Graph，然后将事件总结变成图压缩的问题，提取出Event Graph中最突出的子图作为事件总结。 </details>

* Utilizing Relative Event Time to Enhance Event-Event Temporal Relation Extraction. Haoyang Wen, Heng Ji. EMNLP 2021 Short paper. [Code](https://github.com/wenhycs/EMNLP2021-Utilizing-Relative-Event-Time-to-Enhance-Event-Event-Temporal-Relation-Extraction). <details>  <summary>Details</summary>  Event Temporal Relation Extraction，方法非常简单，就是在两个Event Representation Concatenation的基础上，对两个事件的相对顺序进行显式建模，为事件打上相对时序标签（前面的事件为-1，后面的事件为1），然后把相对时间预测和时序关系抽取结合在一起进行训练。 </details>

* Event Time Extraction and Propagation via Graph Attention Networks. Haoyang Wen, Yanru Qu, Heng Ji, Qiang Ning, Jiawei Han, Avi Sil, Hanghang Tong, Dan Roth. NAACL 2021 Full paper. [Code](https://github.com/wenhycs/NAACL2021-Event-Time-Extraction-and-Propagation-via-Graph-Attention-Networks). <details>  <summary>Details</summary>  不同于通常的Event Temporal Relation Extraction，本文提出基于文档中具有时间信息的相关事件来预测目标事件的绝对时间（包括最早发生时间、最晚发生时间、最早结束时间、最晚结束时间）。利用Argument相同和自动事件时序关系抽取来构建文档级别的事件图，然后采用GAT来进行建模。具体模型细节没看。 </details>

* EventPlus: A Temporal Event Understanding Pipeline. Mingyu Derek Ma, Jiao Sun, Mu Yang, Kung-Hsiang Huang, Nuan Wen, Shikhar Singh, Rujun Han, Nanyun Peng. NAACL 2021 Full paper. [Code](https://github.com/PlusLabNLP/EventPlus). <details>  <summary>Details</summary>  相当于是Event相关的一个系统，包含了event trigger and type detection, event argument detection, event duration and temporal relation extraction。具体细节没看。 </details>

* Temporal Reasoning on Implicit Events from Distant Supervision. Ben Zhou, Kyle Richardson, Qiang Ning, Tushar Khot, Ashish Sabharwal, Dan Roth. NAACL 2021 Full paper. [Code](https://github.com/allenai/tracie). <details>  <summary>Details</summary>  以往的Temporal Relation Extraction工作都是基于显式事件进行事件排序，但文本中可能存在一些隐式事件。因此，本文构造了一个包含隐式事件的数据集，并且提出A distant supervision process来进行隐式事件的排序，以及提出通过预测事件的start time和duration来判断事件的结束时间。具体模型细节没看。 </details>

* Time-Stamped Language Model: Teaching Language Models to Understand The Flow of Events. Hossein Rajaby Faghihi, Parisa Kordjamshidi. NAACL 2021 Full paper. [Code](https://github.com/HLR/TSLM). <details>  <summary>Details</summary>  本文目的和【21 EMNLP ECONET Effective Continual Pretraining of Language Models for Event Temporal Reasoning】非常相似，解决当前预训练模型难以建模事件流的问题。以往方法均是通过改变模型输入来考虑不同Step，本文提出把该问题当作QA问题来处理，当作QA问题就可以利用其他QA benchmark来帮助进行文本理解，本文无需改变模型输入。具体模型细节没看。 </details>

* Discourse-Level Event Temporal Ordering with Uncertainty-Guided Graph Completion. Jian Liu, Jinan Xu, Yufeng Chen, Yujie Zhang. IJCAI 2021. [Code](https://github.com/jianliu-ml/EventTemp). <details>  <summary>Details</summary>  Event Temporal Relation Extraction，提出将document构造成temporal graph，每个节点是一个event，每个边是event间的关系，从而可以学习global features和inter-dependencies。具体来说，首先采用BiLSTM编码Event作为node表示，然后采用R-GCN来进行信息传播更新node表示，最后预测两个事件间的关系。另外，在进行预测时，由于事件间的关系都不知道，导致事件图为empty graph，本文提出Uncertainty-Guided Graph Completion（具体细节没看）来解决该问题。 </details>

* Distinguishing Between Foreground and Background Events in News. Mohammed Aldawsari, Adrián Pérez, Deya Banisakher, Mark A. Finlayson. COLING 2020 Full paper. <details>  <summary>Details</summary>  定义了一种新的task，区分article中事件是否为foreground events，还是background events，或者其他，并且判断background event与foreground event的关系。（We define foreground events as those that comprise the main topic of a news article, as indicated by the headline. In contrast, background events add supporting or contextual information.） </details>

* Domain Knowledge Empowered Structured Neural Net for End-to-End Event Temporal Relation Extraction. Rujun Han, Yichao Zhou, Nanyun Peng. EMNLP 2020 Full paper. <details>  <summary>Details</summary>  Event Temporal Relation Extraction，两个数据集TimeBank-Dense（时序关系包括BEFORE,AFTER, INCLUDES, INCLUDED, SIMULTANEOUS, and VAGUE）和I2B2-TEMPORAL（时序关系包括BEFORE, AFTER, and OVERLAP）。以往方法面临强约束在现实场景下不准确，以及数据集较小的问题，因此本文提出在模型推理时引入领域知识来缓解数据集较小的问题，以及采用Lagrangian Relaxation来解决约束推理问题。另外本文的任务定义是先从文本中检测出事件，然后判定每两个事件间的时序关系，是一个端到端的模型。具体模型细节没看。 </details>

* Severing the Edge Between Before and After: Neural Architectures for Temporal Ordering of Events. Miguel Ballesteros, Rishita Anubhai, Shuai Wang, Nima Pourdamghani, Yogarshi Vyas, Jie Ma, Parminder Bhatia, Kathleen R. McKeown, Yaser Al-Onaizan. EMNLP 2020 Full paper. <details>  <summary>Details</summary>  Event Temporal Relation Extraction，主要包括以下几点贡献：（1）灵活采用不同编码器来编码event；（2）采用Scheduled Multitask-Learning方法，利用互补的数据（包括时序的和非时序的），仿照预训练和微调；（3）自学习方法，首先训练一个模型，用该模型去标注无标签数据，然后再用这些自动标注的数据去进行训练。迭代训练。 </details>
