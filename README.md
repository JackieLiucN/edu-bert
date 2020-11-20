# 好未来开源教育领域首个在线教学中文预训练模型TAL-EduBERT

## 一、背景及下载地址

### 1. 背景

2020年初Covid-19疫情的爆发对各行各业产生了不可小觑的影响，也让以线下方式为主的传统教育在短期内受到了极大的冲击，更多人开始看到科技对教育市场的价值。在线教育成为了特殊时期教学的最佳选择，大规模地渗透至每一所学校、每一个家庭。在线教育的爆火使得教育行业产生了海量的在线教学语音识别（Automatic Speech Recognition，以下简称ASR）文本数据，极大地推动了教育领域技术的发展。

数据作为产业最为核心和宝贵的资源之一，更是自然语言处理技术（Natural Language Processing，以下简称NLP）在各个领域得以应用和发展的基础。在线教育文本数据有着区别于通用场景数据的特有属性，给在线教育领域NLP的研究、应用和发展带来了极大的挑战，一是从音视频转录出来的文本数据中，存在着较多的ASR错误，这些错误可能会对文本处理相关任务的效果造成较大的影响；二是数据中含有大量的教育领域特有的专有词汇，现有的通用领域的开源词向量和开源预训练语言模型（如Google BERT Base[1]，Roberta[2]等）对于这些词汇的语义表示能力有限，进而会影响后续任务的效果。

为了帮助解决这两个问题，好未来AI中台机器学习团队从多个来源收集了超过2000万条（约包含3.8亿Tokens）的教育领域中文ASR文本数据，基于此建立了**教育领域首个在线教学中文预训练模型TAL-EduBERT**，并把其推至开源。

从2018年谷歌发布预训练模型BERT以来，以BERT为代表的预训练语言模型， 在各个自然语言处理任务上都达到了SOTA的效果。并且作为通用的预训练语言模型，BERT的出现，使得NLP算法工程师不需要进行繁重的网络结构的修改，直接对于下游任务进行fine-tune，便可得到比以往的深度学习方法更好的效果，显著的减轻了NLP算法工程师的繁重的调整模型网络结构的工作，降低了算法应用的成本，预训练语言模型已经成为工作中不可或缺的一项基础技术。

但是，当前开源的各类中文领域的深度预训练模型，多是面向通用领域的应用需求，在包括教育在内的多个垂直领域均没有看到相关开源模型。相较于谷歌发布的Google BERT Base以及开源的中文Roberta模型，**好未来本次开源的TAL-EduBERT在多个教育领域的下游任务中得到了显著的效果提升**。好未来希望通过本次开源，助力推动 NLP技术在教育领域的应用发展，欢迎各位同仁下载使用。

### 2. 模型下载

下载地址：[https://ai.100tal.com/download/TAL-EduBERT.zip](https://ai.100tal.com/download/TAL-EduBERT.zip)