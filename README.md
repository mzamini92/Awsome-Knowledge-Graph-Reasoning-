# Awsome-Knowledge-Graph-Reasoning 
* [**2022**](#2022-papers)
  - [*NIPS-2022*](#nips-2022)
  - [*AAAI-2022*](#aaai-2022)
  - [*EMNLP-2022*](#emnlp-2022)
  -  [*ICLR-2022*](#iclr-2022)

* [**2021**](#2021-papers) 
  - [*NIPS-2021*](#nips-2021)
  -  [*AAAI-2021*](#aaai-2021)
  -  [*EMNLP-2021*](#emnlp-2021)
  -  [*ICLR-2021*](#iclr-2021)

* [**2020**](#2020-papers) 
  -  [*NIPS-2020*](#nips-2020)
  -  [*EMNLP-2020*](#emnlp-2020)
  -  [*ICLR-2020*](#iclr-2020)
* [**2019**](#2019-papers)
  -  [*NIPS-2019*](#nips-2019)
  -  [*AAAI-2019*](#aaai-2019)
  -  [*EMNLP-2019*](#emnlp-2019)
* [**2018**](#2018-papers)  
  -  [*AAAI-2018*](#aaai-2018)
  -  [*EMNLP-2018*](#emnlp-2018)

# 2022 Papers
## *NIPS-2022*
* [**Learning to Sample and Aggregate: Few-shot Reasoning over Temporal Knowledge Graphs**](https://papers.nips.cc/paper_files/paper/2022/file/6b295b08549c0441914e391651423477-Paper-Conference.pdf)
In this paper, we investigate a realistic but underexplored problem, called few-shot temporal knowledge graph reasoning, that aims to predict future facts for newly emerging entities based on extremely limited observations in evolving graphs. It offers practical value in applications that need to derive instant new knowledge about new entities in temporal knowledge graphs (TKGs) with minimal supervision. The challenges mainly come from the few-shot and time shift properties of new entities. First, the limited observations associated with them are insufficient for training a model from scratch. Second, the potentially dynamic distributions from the initially observable facts to the future facts ask for explicitly modeling the evolving characteristics of new entities. We correspondingly propose a novel Meta Temporal Knowledge Graph Reasoning (MetaTKGR) framework. Unlike prior work that relies on rigid neighborhood aggregation schemes to enhance low-data entity representation, MetaTKGR dynamically adjusts the strategies of sampling and aggregating neighbors from recent facts for new entities, through temporally supervised signals on future facts as instant feedback. Besides, such a meta temporal reasoning procedure goes beyond existing meta-learning paradigms on static knowledge graphs that fail to handle temporal adaptation with large entity variance. We further provide a theoretical analysis and propose a temporal adaptation regularizer to stabilize the meta temporal reasoning over time. Empirically, extensive experiments on three real-world TKGs demonstrate the superiority of MetaTKGR over eight state-of-the-art baselines by a large margin.


## *AAAI-2022*:
* [**TempoQR: Temporal Question Reasoning over Knowledge Graphs**](https://ojs.aaai.org/index.php/AAAI/article/view/20526/20285): TempoQR is a comprehensive embedding-based framework for answering complex questions involving temporal information over Temporal Knowledge Graphs (TKGs). It generates question-specific time embeddings and combines them with entity and context-aware information to ground the question to the specific entities and time scope it refers to. A transformer-based encoder then fuses this temporal information with the question representation for answer predictions. TempoQR was found to significantly improve accuracy and generalize better to unseen question types compared to state-of-the-art approaches. [CODE](https://github.com/cmavro/TempoQR)

* [**Learning to Walk with Dual Agents for Knowledge Graph Reasoning**](https://ojs.aaai.org/index.php/AAAI/article/view/20538/20297): A dual-agent reinforcement learning framework has been developed to improve the accuracy and efficiency of graph walking for reasoning tasks over incomplete knowledge graphs. The approach trains two agents, Giant and Dwarf, to search for answers collaboratively, with Giant searching on cluster-level paths quickly and providing stage-wise hints for Dwarf. Experimental results on several KG reasoning benchmarks showed that the approach outperformed existing RL-based methods for long path queries by a large margin. [CODE](https://github.com/RutgersDM/DKGR/tree/master)

* [**Reasoning about Causal Models with Infinitely Many Variables**](https://ojs.aaai.org/index.php/AAAI/article/view/20508/20267): Generalized structural equations models (GSEMs) are a generalization of structural equations models (SEMs) that can handle infinitely many variables with infinite ranges, which is useful for capturing dynamical systems. A sound and complete axiomatization of causal reasoning in GSEMs has been developed, which extends the sound and complete axiomatization provided by Halpern (2000) for SEMs. This axiomatization helps clarify the properties captured by Halpern's axioms. [CODE](


# 2021 Papers
## *NIPS-2021*
* [**SQALER: Scaling Question Answering by Decoupling Multi-Hop and Logical Reasoning**](https://papers.nips.cc/paper/2021/file/68bd22864919297c8c8a8c32378e89b4-Paper.pdf): A new approach to multi-hop reasoning over knowledge graphs (KGs) has been developed that scales linearly with the number of relation types in the graph, rather than the number of edges or nodes. This allows for more complex logical reasoning without losing expressive power and enables the solution of the multi-hop MetaQA dataset and achievement of a new state-of-the-art on the WebQuestionsSP dataset. The approach is orders of magnitude more scalable than competing methods and can achieve compositional generalization outside of the training distribution.

* [**Leveraging the Inductive Bias of Large Language Models for Abstract Textual Reasoning**](https://papers.nips.cc/paper/2021/file/8e08227323cd829e449559bb381484b7-Paper.pdf): Natural language models, such as GPT-3 and T5, have been found to provide useful inductive bias for training symbolic reasoning engines on nontraditional tasks. These engines demonstrate quick learning and natural generalization that reflects human intuition, such as the ability to generalize blockstacking to stacking other types of objects. The authors also found that compositional learning, where a learner trained on simpler tasks gains an advantage when tackling more complicated tasks, is effective in this context. The study focused on abstract textual reasoning tasks such as object manipulation and navigation, and demonstrated generalization to novel scenarios and symbols.

* [**SalKG: Learning From Knowledge Graph Explanations for Commonsense Reasoning**](https://proceedings.neurips.cc/paper/2021/file/9752d873fa71c19dc602bf2a0696f9b5-Paper.pdf): Saliency methods, which measure how much a knowledge graph (KG) feature influences the model to make a correct prediction, can be used to improve the performance of KG-augmented models on various commonsense reasoning tasks. This paper proposes a framework called SalKG, which uses coarse and fine saliency explanations created from a task's training set to guide the model's attention to useful KG features. SalKG was found to significantly improve performance on three popular commonsense QA benchmarks and a range of KG-augmented models, with up to a 2.76% absolute improvement on CSQA. [CODE](https://github.com/INK-USC/SalKG)

* [**ConE: Cone Embeddings for Multi-Hop Reasoning over Knowledge Graphs**](https://proceedings.neurips.cc/paper/2021/file/a0160709701140704575d499c997b6ca-Paper.pdf): A new technique called ConE has been developed to improve query embedding, which aims to represent entities and first-order logical queries in low-dimensional spaces in order to facilitate multi-hop reasoning over knowledge graphs. ConE is the first geometry-based model that can handle all first-order logical operations, including conjunction, disjunction, and negation. It represents entities and queries as Cartesian products of two-dimensional cones, with the intersection and union of cones representing conjunction and disjunction, and geometric complement operators in the embedding space representing negation. ConE was found to significantly outperform existing state-of-the-art methods on benchmark datasets. [CODE](https://github.com/MIRALab-USTC/QE-ConE)

* [**How to transfer algorithmic reasoning knowledge to learn new algorithms?**](https://papers.nips.cc/paper/2021/file/a2802cade04644083dcde1c8c483ed9a-Paper.pdf): Researchers have studied how to transfer algorithmic reasoning knowledge in order to solve tasks for which only input and output examples are available. They focused on two types of graph algorithms: parallel algorithms such as breadth-first search and Bellman-Ford, and sequential greedy algorithms like Prim and Dijkstra. They created a dataset including nine algorithms and three different graph types and found that standard transfer techniques were not sufficient to achieve systematic generalisation. Instead, they found that multi-task learning can be used to transfer algorithmic reasoning knowledge.

* [**Probabilistic Entity Representation Model for Reasoning over Knowledge Graphs**](https://papers.nips.cc/paper/2021/file/c4d2ce3f3ebb5393a77c33c0cd95dc93-Paper.pdf): A new technique called Probabilistic Entity Representation Model (PERM) has been developed to improve logical reasoning over Knowledge Graphs (KGs). The current approach uses spatial geometries such as boxes to learn query representations, but this has restrictive geometry and leads to non-smooth strict boundaries. PERM encodes entities as a Multivariate Gaussian density with mean and covariance parameters to capture its semantic position and smooth decision boundary, respectively. It also defines closed logical operations of projection, intersection, and union that can be aggregated using an end-to-end objective function. The technique was found to significantly outperform state-of-the-art methods on various benchmark KG datasets and was able to recommend drugs with better F1 scores in a COVID-19 drug-repurposing case study. The working of the query answering process was also demonstrated through a low-dimensional visualization of the Gaussian representations. [CODE](https://github.com/Akirato/PERM-GaussianKG)

## *AAAI-2021:*
* [**KG-BART: Knowledge Graph-Augmented BART for Generative Commonsense Reasoning**](https://ojs.aaai.org/index.php/AAAI/article/view/16796/16603): KG-BART is a novel knowledge graph augmented pre-trained language generation model that incorporates the complex relations of concepts through a knowledge graph to produce more logical and natural sentences. It leverages graph attention to aggregate the rich concept semantics, improving generalization on unseen concept sets. Experiments on the CommonGen dataset show that KG-BART outperforms other pre-trained language generation models, particularly BART, in terms of BLEU scores. KG-BART's generated context can also be used as background scenarios to benefit downstream commonsense QA tasks. [CODE](https://github.com/yeliu918/KG-BART)
## *EMNLP-2021:*
* [CR-Walker: Tree-Structured Graph Reasoning and Dialog Acts for Conversational Recommendation](https://aclanthology.org/2021.emnlp-main.139.pdf): In this paper, the authors propose CR-Walker, a model for conversational recommender systems that can perform tree-structured reasoning on a knowledge graph and generate informative dialog acts to guide language generation. The model is designed to improve the ability to introduce relevant items and attributes and arrange selected entities appropriately under current system intents. Automatic and human evaluations show that CR-Walker can achieve more accurate recommendations and generate more informative and engaging responses. [CODE](https://github.com/truthless11/CR-Walker)

*  [GMH: A General Multi-hop Reasoning Model for KG Completion](https://aclanthology.org/2021.emnlp-main.276.pdf): Multi-hop reasoning over knowledge graphs is a challenging task, particularly when it comes to long-distance reasoning. Current models are limited in their ability to connect superficially unrelated entities. This paper proposes a general framework for multi-hop reasoning that addresses two key issues: where to go and when to stop. The proposed model includes three modules: a local-global knowledge module to estimate possible paths, a differentiated action dropout module to explore a diverse set of paths, and an adaptive stopping search module to avoid over searching. The model is tested on three datasets and demonstrates superior performance, particularly in long-distance reasoning scenarios.
*  [CRFR: Improving Conversational Recommender Systems via Flexible Fragments Reasoning on Knowledge Graphs](https://aclanthology.org/2021.emnlp-main.355.pdf): In this paper, the authors propose CRFR, a conversational recommender system that uses a reinforcement learning model to perform multi-hop reasoning on knowledge graphs in order to better understand user interests and make recommendations. CRFR is designed to handle incomplete knowledge graphs and learn multiple reasoning fragments instead of complete paths. The system also uses a unified model to fuse information from item- and concept-oriented knowledge graphs to improve the response of the CRS. Experiments show that CRFR performs well in recommendation, conversation, and conversation interpretability.

* [Is Multi-Hop Reasoning Really Explainable? Towards Benchmarking Reasoning Interpretability](https://aclanthology.org/2021.emnlp-main.700.pdf): In summary, this paper presents a framework for evaluating the interpretability of multi-hop reasoning models in link prediction tasks. The proposed framework includes three metrics for path recall, local interpretability, and global interpretability. The effectiveness of the framework is demonstrated through experiments with nine representative baselines, which show that the interpretability of current multi-hop reasoning models is relatively low and there is room for improvement. The results also suggest that rule-based models may be a promising direction for future research in this area. [CODA](https://github.com/THU-KEG/BIMR)

* [UniKER: A Unified Framework for Combining Embedding and Definite Horn Rule Reasoning for Knowledge Graph Inference](https://aclanthology.org/2021.emnlp-main.769.pdf): The problem of performing complex multi-hop logical reasoning over knowledge graphs (KGs) has been a challenge in artificial intelligence. Recent approaches have used KG embeddings to find answers, but have been limited in their ability to handle certain first-order logic operators, such as negation, and are unable to naturally model uncertainty. A new method called BetaE has been proposed that uses probabilistic distributions with bounded support, specifically the Beta distribution, to embed queries and entities as distributions and perform logical operations using neural operators. BetaE is able to handle all first-order logical operations and model uncertainty, and is shown to be more effective than current state-of-the-art KG reasoning methods on three large, incomplete KGs.

## *ICLR-2022*:
[GreaseLM: Graph REASoning Enhanced Language Models ](https://openreview.net/pdf?id=41e9o6cQPj): GreaseLM is a new model that aims to improve the ability of question answering systems to perform complex reasoning by fusing encoded representations from pretrained language models and graph neural networks over multiple layers of modality interaction operations. The goal is to allow language context representations to be grounded in structured world knowledge and to allow linguistic nuances in the context to inform the graph representations of knowledge. The model is tested on three benchmarks in the commonsense reasoning and medical question answering domains and is found to be able to more reliably answer questions that require reasoning over both situational constraints and structured knowledge, outperforming models that are 8 times larger.

## *ICLR-2021*: 
[RNNLogic: Learning Logic Rules for Reasoning on Knowledge Graphs](https://openreview.net/pdf?id=tGZu6DlbreV): RNNLogic is a probabilistic model for learning logic rules for reasoning on knowledge graphs. It treats logic rules as a latent variable and simultaneously trains a rule generator and a reasoning predictor with logic rules. RNNLogic uses an EM-based algorithm to optimize the model, where the reasoning predictor is updated to explore generated logic rules for reasoning and a set of high-quality rules is selected through posterior inference using both the rule generator and reasoning predictor. Experiments on four datasets show that RNNLogic is effective for knowledge graph reasoning. [CODE](https://github.com/DeepGraphLearning/RNNLogic)

[Explainable Subgraph Reasoning for Forecasting on Temporal Knowledge Graphs](https://openreview.net/pdf?id=pGIHq1m7PU): This paper presents a framework for predicting links in time-evolving knowledge graphs (KGs) that focuses on interpreting predictions by reasoning over query-relevant subgraphs and jointly modeling structural dependencies and temporal dynamics. The proposed approach includes a temporal relational attention mechanism and a reverse representation update scheme to guide the extraction of a subgraph around the query and expand it through iterative sampling and attention propagation. Evaluation on four benchmark temporal KGs shows improved performance and explainability compared to the previous best temporal KG forecasting method. The approach also receives positive feedback from a survey of 53 respondents on its alignment with human understanding.

[RNNLogic: Learning Logic Rules for Reasoning on Knowledge Graphs](https://openreview.net/pdf?id=tGZu6DlbreV): RNNLogic is a probabilistic model for learning interpretable logic rules for reasoning on knowledge graphs. It uses an Expectation-Maximization (EM) based algorithm to optimize the rule generator and reasoning predictor simultaneously. RNNLogic treats logic rules as a latent variable and trains both the rule generator and reasoning predictor with logic rules. In each iteration, the reasoning predictor is updated to explore some generated logic rules for reasoning, and the rule generator is updated with a set of high-quality rules selected from all generated rules through posterior inference. Experiments on four datasets show that RNNLogic is effective in learning interpretable logic rules for reasoning on knowledge graphs. [CODE](https://github.com/DeepGraphLearning/RNNLogic)


# 2020 Papers
## *NIPS-2020*:
* [**Beta Embeddings for Multi-Hop Logical Reasoning in Knowledge Graphs**](https://papers.nips.cc/paper/2020/file/e43739bba7cdb577e9e3e4e42447f5a5-Paper.pdf): Artificial intelligence researchers have developed a method called BetaE that can handle complex multi-hop logical reasoning over knowledge graphs (KGs). BetaE is the first approach that can handle all first-order logical operations, including conjunction, disjunction and negation, while also being able to model uncertainty. It uses probabilistic distributions with bounded support, specifically the Beta distribution, to embed queries and entities as distributions and performs logical operations in the embedding space using neural operators. BetaE was tested on three large, incomplete KGs and was found to increase relative performance by up to 25.4% over current state-of-the-art KG reasoning methods that can only handle conjunctive queries without negation.

* [**Duality-Induced Regularizer for Tensor Factorization Based Knowledge Graph Completion**](https://papers.nips.cc/paper/2020/file/f6185f0ef02dcaec414a3171cd01c697-Paper.pdf): A new regularizer called DURA has been developed to address the overfitting problem in tensor factorization-based models for knowledge graph completion. DURA is based on the observation that for an existing tensor factorization model, there is often another distance-based model closely associated with it. It is effective in improving the performance of existing models and widely applicable to various methods. [CODE](https://github.com/MIRALab-USTC/KGE-DURA)
## *EMNLP-2020*
* [Learning Collaborative Agents with Rule Guidance for Knowledge Graph Reasoning](https://aclanthology.org/2020.emnlp-main.688.pdf): In summary, RuleGuider is a method that combines symbolic and walk-based approaches for knowledge graph reasoning by using rules generated by symbolic methods to guide walk-based reinforcement learning models. It has been shown to improve the performance of walk-based models without sacrificing interpretability. [CODE](https://github.com/derenlei/KG-RuleGuider)

* [Dynamic Anticipation and Completion for Multi-Hop Reasoning over Sparse Knowledge Graph](https://aclanthology.org/2020.emnlp-main.459.pdf): In summary, DacKGR is a multi-hop reasoning model for knowledge graph completion that utilizes dynamic anticipation and completion strategies to improve performance on sparse KGs. The anticipation strategy uses latent prediction of embedding-based models to perform potential path search, while the completion strategy dynamically adds edges as additional actions to alleviate the sparseness of the KG. The model is tested on five datasets and outperforms state-of-the-art baselines. [CODE](https://github.com/THU-KEG/DacKGR)
* [Scalable Multi-Hop Relational Reasoning for Knowledge-Aware Question Answering](https://aclanthology.org/2020.emnlp-main.99.pdf): In this paper, the authors propose a new approach for augmenting question answering models with external knowledge, such as knowledge graphs, by using a multi-hop graph relation network (MHGRN). The MHGRN is designed to perform multi-hop, multi-relational reasoning over subgraphs extracted from knowledge graphs, combining path-based reasoning methods and graph neural networks for improved interpretability and scalability. The authors demonstrate the effectiveness and scalability of their approach on CommonsenseQA and OpenbookQA datasets and provide case studies to interpret the behavior of their model.[CODE](https://github.com/INK-USC/MHGRN)
* [Language Generation with Multi-Hop Reasoning on Commonsense Knowledge Graph](https://aclanthology.org/2020.emnlp-main.54.pdf): GRF is a model that enhances pre-trained language models with the ability to perform multi-hop reasoning over multi-relational paths in external knowledge graphs. This helps to improve text generation in cases where reasoning over commonsense knowledge is necessary. GRF has been shown to outperform existing baselines on three text generation tasks that require commonsense knowledge, and its effectiveness is demonstrated through the inference of reasoning paths that provide rationale for the generation. [CODE](https://github.com/cdjhz/multigen)
## *ICLR-2020*:
* [Learning to Retrieve Reasoning Paths over Wikipedia Graph for Question Answering](http://www.openreview.net/pdf?id=SJgVHkrYDH): The authors propose a graph-based approach to answering multi-hop open-domain questions by retrieving reasoning paths from the Wikipedia graph. They use a recurrent neural network to sequentially retrieve evidence paragraphs and a reader model to rank the reasoning paths and extract the answer span from the best path. The approach shows state-of-the-art results on three open-domain QA datasets, including a significant improvement on HotpotQA. [CODE](https://github.com/AkariAsai/learning_to_retrieve_reasoning_paths)
* [Query2box: Reasoning over Knowledge Graphs in Vector Space Using Box Embeddings](http://www.openreview.net/pdf?id=BJgr4kSFDS): query2box is a new approach for performing complex logical queries on large, incomplete knowledge graphs. It allows for the use of multiple logical operators, including conjunction, disjunction, and existential quantifiers, and represents queries as boxes in a vector space. By transforming queries into Disjunctive Normal Form, query2box can handle arbitrary logical queries in a scalable manner and has shown up to 25% relative improvement over existing methods on two large knowledge graphs. [CODE](https://github.com/hyren/query2box)

* [Dynamically Pruned Message Passing Networks for Large-scale Knowledge Graph Reasoning](http://www.openreview.net/pdf?id=rkeuAhVKvB): The authors propose Dynamically Pruned Message Passing Networks (DPMPN) for large-scale knowledge graph reasoning. DPMPN learns an input-dependent subgraph to model a sequential reasoning process, which is constructed dynamically and expands selectively under a flow-style attention mechanism. This allows the model to not only provide graphical explanations for predictions, but also prune message passing in Graph Neural Networks (GNNs) to scale with the size of graphs. The authors take inspiration from the concept of consciousness prior proposed by Bengio to design a two-GNN framework that encodes global input-invariant graph-structured representation and learns local input-dependent representation coordinated by an attention module. Experiments show that DPMPN outperforms state-of-the-art methods in knowledge base completion tasks and has strong reasoning capabilities.[CODE](https://github.com/hyren/query2box)
# 2019 Papers
## *NIPS-2019*:
* [DRUM: End-To-End Differentiable Rule Mining On Knowledge Graphs](https://papers.nips.cc/paper/2019/file/0c72cb7ee1512f800abe27823a792d03-Paper.pdf): DRUM is a scalable and differentiable approach for mining first-order logical rules from knowledge graphs for inductive link prediction. It is motivated by the connection between learning confidence scores for each rule and low-rank tensor approximation and uses bidirectional RNNs to share information across tasks. DRUM was found to be more efficient than existing rule mining methods for inductive link prediction on various benchmark datasets.

## *AAAI-2019*:
* [Explainable Reasoning over Knowledge Graphs for Recommendation](https://ojs.aaai.org/index.php/AAAI/article/view/4470/4348): Incorporating knowledge graphs into recommender systems has gained popularity in recent years due to their ability to explore the connectivity between users and items as paths, providing rich and complementary information beyond traditional user-item interactions. These paths not only reveal the semantics of entities and relations, but also help to understand a user's interests. However, current approaches have not fully utilized this connectivity to infer user preferences, particularly in terms of modeling the sequential dependencies and holistic semantics of a path.
## *EMNLP-2019*: 
* [Knowledge Aware Conversation Generation with Explainable Reasoning over Augmented Graphs](https://aclanthology.org/D19-1187.pdf): In summary, this research proposes a new method for open domain conversation generation that combines knowledge from both knowledge graphs and texts. The method uses multi-hop graph reasoning to effectively select relevant knowledge for conversation and incorporates machine reading comprehension technology to make use of long text information. The method is evaluated on two datasets and shown to outperform existing state-of-the-art models. [CODE](https://github.com/PaddlePaddle/Research/tree/master/NLP/EMNLP2019-AKGCM)
* [Incorporating Graph Attention Mechanism into Knowledge Graph Reasoning Based on Deep Reinforcement Learning](https://aclanthology.org/D19-1264.pdf): There has been growing interest in using knowledge graphs (KGs) to improve artificial intelligence (AI) systems, particularly in the area of multi-hop logical reasoning over large and incomplete KGs. However, current approaches have limitations, such as being unable to handle all first-order logic operators and modeling uncertainty. To address these issues, a new probabilistic embedding framework called BetaE has been proposed. BetaE uses a Beta distribution to embed queries and entities as distributions and allows for the handling of all first-order logic operations, including conjunction, disjunction, and negation. It also allows for the natural modeling of uncertainty. BetaE has been tested on three large, incomplete KGs and has shown improved performance over current state-of-the-art KG reasoning methods, which are limited to conjunctive queries without negation.

* [DIVINE: A Generative Adversarial Imitation Learning Framework for Knowledge Graph Reasoning](https://aclanthology.org/D19-1266.pdf): There is a growing interest in using knowledge graphs (KGs) to improve artificial intelligence (AI) systems, but these systems often struggle with multi-hop logical reasoning and handling incomplete or large KGs. Many studies have proposed using embedding techniques and probabilistic distributions, as well as reinforcement learning and generative adversarial imitation learning, to address these challenges. These methods aim to allow AI systems to perform complex multi-hop reasoning, handle arbitrary first-order logic queries and uncertainty, and improve their performance on tasks such as question answering and text generation. Some approaches have also focused on incorporating symbolic reasoning methods and interpretability measures to better understand the reasoning process. These methods have been applied to a variety of knowledge graphs, including Freebase, NELL, and Wikidata, and have shown promising results in terms of performance and efficiency.

* [Collaborative Policy Learning for Open Knowledge Graph Reasoning](https://aclanthology.org/D19-1269.pdf): There is a growing interest in using knowledge graphs for artificial intelligence tasks, particularly in multi-hop logical reasoning and question answering. However, these tasks are challenging due to the size and incompleteness of knowledge graphs. Several approaches have been developed to embed knowledge graph entities in a low-dimensional space and use these embeddings to find answers, but these methods have limitations, including a lack of support for the negation operator and the inability to naturally model uncertainty. A new method called BetaE has been proposed that uses probabilistic embeddings and neural operators to handle all first-order logical operations, including conjunction, disjunction, and negation, and also allows for the modeling of uncertainty. BetaE has been tested on three large, incomplete knowledge graphs and has shown improved performance compared to current state-of-the-art methods. [CODE](https://github.com/INK-USC/CPL)

* [Adapting Meta Knowledge Graph Information for Multi-Hop Reasoning over Few-Shot Relations](https://aclanthology.org/D19-1334.pdf): In this research, the problem of multi-hop reasoning in knowledge graphs is addressed. It is a challenge to build systems that can perform complex logical reasoning over knowledge graphs, because these graphs can be large and incomplete. The authors propose a probabilistic embedding framework called BetaE, which can handle a full set of first-order logical operations, including conjunction, disjunction, and negation. BetaE uses probabilistic distributions with bounded support, specifically the Beta distribution, and embeds queries and entities as distributions, allowing it to model uncertainty. Logical operations are performed in the embedding space by neural operators over the probabilistic embeddings. BetaE is tested on three large, incomplete knowledge graphs and performs well, with a 25.4% increase in relative performance over current state-of-the-art methods. [CODE](https://github.com/THU-KEG/MetaKGR)
* [Self-Assembling Modular Networks for Interpretable Multi-Hop Reasoning](https://aclanthology.org/D19-1455.pdf): Artificial intelligence researchers are working on ways to use knowledge graphs to perform complex multi-hop logical reasoning, which can be challenging due to the size and incompleteness of knowledge graphs. One approach is to use probabilistic embeddings, specifically Beta distributions, to embed queries and entities in a low-dimensional space and perform logical operations with neural operators. This approach, called BetaE, can handle all first-order logical operations, including conjunction, disjunction, and negation, and can model uncertainty. BetaE has been tested on three large knowledge graphs and has demonstrated an improvement of up to 25.4% over state-of-the-art methods that can only handle conjunctive queries without negation. Other approaches for improving knowledge graph reasoning include using tree-structured reasoning and generating informative dialog acts, using a unified framework that combines knowledge graph embedding with logical rules, using a deep reinforcement learning model with memory components to improve performance and efficiency, using a plug-and-play framework based on generative adversarial imitation learning to enhance existing reinforcement learning methods, and using meta-learning to adapt to few-shot relations in knowledge graphs. [CODE](https://github.com/jiangycTarheel-zz/NMN-MultiHopQA)
 

# 2018 Papers

## *AAAI-2018*: 
* [Variational Reasoning for Question Answering with Knowledge Graph](https://ojs.aaai.org/index.php/AAAI/article/view/12057/11916): A new approach for question answering (QA) using knowledge graphs (KGs) has been proposed, which aims to handle noisy questions and perform multi-hop reasoning simultaneously. The method uses a deep learning architecture and an end-to-end variational learning algorithm to achieve state-of-the-art performance on a benchmark dataset. The approach has also been tested on several new benchmark datasets, including questions requiring multi-hop reasoning, paraphrased questions, and questions in human voice, and has shown promising results.
## *EMNLP-2018*
* [Multi-Hop Knowledge Graph Reasoning with Reward Shaping](https://aclanthology.org/D18-1362.pdf): There has been a recent focus on the use of artificial intelligence and machine learning techniques for multi-hop logical reasoning over knowledge graphs (KGs). Current approaches typically embed KG entities in a low dimensional space and use these embeddings to find answer entities, but are limited in their ability to handle arbitrary first-order logic (FOL) queries and uncertainty. In this research, a new probabilistic embedding framework called BetaE was developed to handle arbitrary FOL queries and uncertainty over KGs. BetaE is the first method that can handle all FOL operations, including conjunction, disjunction, and negation, and can model uncertainty through the use of probabilistic distributions with bounded support. The performance of BetaE was demonstrated on three large, incomplete KGs, and it increased relative performance by up to 25.4% compared to state-of-the-art KG reasoning methods that can only handle conjunctive queries without negation. [CODE](https://github.com/salesforce/MultiHopKG)
