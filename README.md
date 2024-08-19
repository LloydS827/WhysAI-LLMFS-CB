![240624_llm_roadmap.drawio](./assets/240624_llm_roadmap.drawio.png)

### Description

WhysAI--**LLMFS**项目是由一系列mini-projects组成、围绕大模型主题的系列课程。主要包括三个系列：

1. [CB(This Repo)](https://github.com/LloydS827/WhysAI-LLMFS-CB)：深度学习基础，包括神经网络、反向传播、PyTorch等；
2. [4S](https://github.com/LloydS827/WhysAI-LLMFS-4S)：以从零到一训练/微调大语言模型为核心；
3. [4E](https://github.com/LloydS827/WhysAI-LLMFS-4E)：以LLM应用为核心，涵盖RAG、Agent、MAS、Inference等。

本项目受到许多优秀的开源课程与资料启发，制作的课程资料包括Slides、Code、Video等，既用来记录学习现代人工智能技术的过程，又希望与大家共同探索AI技术的最佳学习路径。

### CB(Common Basis)系列课程内容（V1.0）
>系列说明：以三个项目作为主体，1）使用Python从零构建MLP，解决MNist问题；2）从零构建针对标量的自动微分架构；3）使用PyTorch构建MLP，解决MNist问题。同时在开始和结尾补充两次理论介绍：1）AI历史；2）AI Career与学习方法。

| Theme & Contents                                             | Course Code & Materials                                      | Project & Keywords                  | Videos                                                       | References                                                   |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ----------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| 1. A Brief History: CB01介绍人工智能简要历史与发展历程，包括起源、达特茅斯会议、三大主义，以及机器学习、深度学习和现代人工智能 | [CB01](https://github.com/LloydS827/WhysAI-LLMFS-CB/tree/main/01_AI) | /                                   | [bilibili](https://www.bilibili.com/video/BV1Hz3xeaEa6/?spm_id_from=333.337.search-card.all.click&vd_source=11cbe4e223f3ef3e00cac82a0cb79098),[youtube](https://www.youtube.com/watch?v=wfMV2kWjElg&t=1s) | 1. [The Bitter Lesson](http://www.incompleteideas.net/IncIdeas/BitterLesson.html)by Rich Sutton<br>2. [智慧的疆界 (豆瓣) (douban.com)](https://book.douban.com/subject/30379536/)<br>3. [人工智能（第4版） (豆瓣) (douban.com)](https://book.douban.com/subject/36152133/)<br>4. [我看见的世界 (豆瓣) (douban.com)](https://book.douban.com/subject/36672955/) |
| 2.1 NN 0-1：CB02-1以三次抽象为核心，从理论上介绍神经网络、梯度下降与反向传播，从而帮助理解现代人工智能技术的核心。 | [CB02-1](https://github.com/LloydS827/WhysAI-LLMFS-CB/tree/main/02-1_NN&BP) | P1: MNist \| MLP \| Python (theory) | [bilibili](https://www.bilibili.com/video/BV1n3hhedEgE/?spm_id_from=333.337.search-card.all.click&vd_source=11cbe4e223f3ef3e00cac82a0cb79098),[youtube](https://www.youtube.com/watch?v=6gDrrDTGLzA&t=1s) | **Main Refs:**<br>1. Michael A. Nielsen, '[Neural networks and deep learning](http://neuralnetworksanddeeplearning.com/chap1.html)', [Github Repo](https://github.com/mnielsen/neural-networks-and-deep-learning/tree/master)<br>2.  The first 3/4 videos in 3B1B’s [“Neural networks”](https://space.bilibili.com/88461692/channel/seriesdetail?sid=1528929)) series.<br>3. Video Lecture on [MicroGrad](https://www.bilibili.com/video/BV1aB4y13761/?spm_id_from=333.337.search-card.all.click&vd_source=11cbe4e223f3ef3e00cac82a0cb79098) By Andrej Karpathy<br>4. [Computational Graph on BP](https://colah.github.io/posts/2015-08-Backprop/) from Chris Olah<br><br>**Others:** <br>1. Chapters 3-5 of the [d2l.ai](http://d2l.ai/) <br>2. [Neural Networks from Scratch in Python Book (nnfs.io)](https://nnfs.io/)<br>3. CS231n's [Python Numpy Tutorial (with Jupyter and Colab) (cs231n.github.io)](https://cs231n.github.io/python-numpy-tutorial/)<br>4. Numpy Tutorial: [Iris  Series Book 1《编程不难》](https://github.com/Visualize-ML/Book1_Python-For-Beginners): C13-C18<br>5. [An efficient pure-PyTorch implementation of KAN](https://github.com/Blealtan/efficient-kan/tree/master)<br>6. [NN SVG (alexlenail.me)](https://alexlenail.me/NN-SVG/index.html) |
| 2.2 NN w/ numpy：CB02-2基于前一课程理论内容，使用Python与Numpy，从零构建MLP，实现Mini-batch SGD优化发放与反向传播机制，进而解决Mnist手写数字识别问题。 | [CB02-2](https://github.com/LloydS827/WhysAI-LLMFS-CB/tree/main/02-2_NN%26BP%20Implementation) | P1: MNist \| MLP \| Python (code)   | [bilibili](https://www.bilibili.com/video/BV1cZbpeeEi3/?spm_id_from=333.337.search-card.all.click&vd_source=11cbe4e223f3ef3e00cac82a0cb79098),[youtube](https://www.youtube.com/watch?v=Tx2akzADo-A) | 1. Michael A. Nielsen, '[Neural networks and deep learning](http://neuralnetworksanddeeplearning.com/chap1.html)', [Github Repo](https://github.com/mnielsen/neural-networks-and-deep-learning/tree/master) |
| 2.3 Autograd：CB02-3针对反向传播算法中的核心问题（计算图与微分），使用纯Python构建小型自动微分引擎，帮助理解反向传播原理与深度学习架构核心 | [CB02-3](https://github.com/LloydS827/WhysAI-LLMFS-CB/tree/main/02-3_Autograd) | P2: Scalar Autograd                 | Part A: [bilibili](https://www.bilibili.com/video/BV1gs8FeQEm1/?spm_id_from=333.337.search-card.all.click),[youtube](https://www.youtube.com/watch?v=wKwOvGzswws)<br><br>Part B: [bilibili](https://www.bilibili.com/video/BV1NpezecE5p/?spm_id_from=333.337.search-card.all.click&vd_source=11cbe4e223f3ef3e00cac82a0cb79098),[youtube](https://www.youtube.com/watch?v=8oJCPYua5qU) | 1. [Andrej Karpathy \| micrograd](https://www.bilibili.com/video/BV1aB4y13761/?spm_id_from=333.337.search-card.all.click) |
| 2.4 Pytorch：CB02-4介绍Pytorch核心组件与典型使用方法，快速上手Pytorch、理解核心特征与功能。最后使用Pytorch复现Mnist案例(CB02-2) | [CB02-4](https://github.com/LloydS827/WhysAI-LLMFS-CB/tree/main/02-4_Pytorch) | P3: MNist \| MLP \| PyTorch         | Part A: [bilibili](https://www.bilibili.com/video/BV17qiMeTE8n/?spm_id_from=333.999.0.0&vd_source=11cbe4e223f3ef3e00cac82a0cb79098), [YouTube](https://www.youtube.com/watch?v=lvSPXpnjMKQ)<br />Part B:[bilibili](https://www.bilibili.com/video/BV1JDYueiEaZ/?spm_id_from=333.999.0.0&vd_source=11cbe4e223f3ef3e00cac82a0cb79098), [youtube](https://www.youtube.com/watch?v=rQgR5FfTTOg) | 1. PyTorch Official Tutorial: [Introduction to PyTorch](https://pytorch.org/tutorials/beginner/introyt.html)<br>2. Appendix A of [LLMs-from-scratch](https://github.com/rasbt/LLMs-from-scratch)<br>3. [Learn the Basics — PyTorch Tutorials](https://pytorch.org/tutorials/beginner/basics/intro.html)<br>4.[What is torch.nn really? — PyTorch Tutorials](https://pytorch.org/tutorials/beginner/nn_tutorial.html#closing-thoughts)<br>5.[cs230-stanford: Code examples in pyTorch and Tensorflow ](https://github.com/cs230-stanford/cs230-code-examples) |
| 3. A Career In AI: 关于AI领域的学习、项目、职业经验与建议-1）持续有深度地完成项目；2）用自己的话总结所学；3）只和自己比较。 | [CB03](https://github.com/LloydS827/WhysAI-LLMFS-CB/tree/main/03_A%20Career%20In%20AI) | /                                   | [bilibili](https://www.bilibili.com/video/BV1wGeMeqEGA/?spm_id_from=333.337.search-card.all.click&vd_source=11cbe4e223f3ef3e00cac82a0cb79098), [YouTube](https://www.youtube.com/watch?v=kXjDpYYsYjo) | For Fundamentals:<br>1. [AI Python for Beginners - DeepLearning.AI](https://www.deeplearning.ai/short-courses/ai-python-for-beginners/)<br>2. [30 days of Python ](https://github.com/Asabeneh/30-Days-Of-Python)<br>3. [Visualize-ML](https://github.com/Visualize-ML)<br>4. [3Blue1Brown的个人空间](https://space.bilibili.com/88461692?spm_id_from=333.337.0.0)<br>5. [课程安排 - 动手学深度学习课程 (d2l.ai)](https://courses.d2l.ai/zh-v2/)<br><br>For Career:<br>1. [How to Build Your Career in AI eBook - Andrew Ng Collected Insights (deeplearning.ai)](https://info.deeplearning.ai/how-to-build-a-career-in-ai-book)<br>2. Musk's Five Steps<br>3. [Karpathy's Speech at Berkeley](https://www.bilibili.com/video/BV1CT421r7oL/?spm_id_from=333.337.search-card.all.click)4. The "WRB" book:[- WRB (whereresearchbegins.com)](https://whereresearchbegins.com/)<br>5. "How Big Things Get Done"[怎样做成大事 (豆瓣) (douban.com)](https://book.douban.com/subject/36827775/)<br>6. [为什么伟大不能被计划](https://book.douban.com/subject/36357804/) [(](https://book.douban.com/subject/36357804/)[豆瓣](https://book.douban.com/subject/36357804/)[) (douban.com)](https://book.douban.com/subject/36357804/) |



### Key Resources

> 每期参考/推荐资料见“课程内容”

**Key Roadmap & Resources:**

- [GenAI Handbook (genai-handbook.github.io)](https://genai-handbook.github.io/)
- [https://github.com/mlabonne/llm-course](https://github.com/mlabonne/llm-course)
- [karpathy/LLM101n: LLM101n: Let's build a Storyteller (github.com)](https://github.com/karpathy/LLM101n)

**Important：**

- [StatQuest](https://space.bilibili.com/3546620985608836?spm_id_from=333.337.0.0)
- Deeplearning.ai
- Andrej Karparthy: Zero 2 Hero Series
- 3B1B: NN series
- VisualizeML(Iris Series)

**Others**：

- AI Infrastructure [https://github.com/chenzomi12/AISystem/](https://github.com/chenzomi12/AISystem/)
- ML-data engineering [https://github.com/GokuMohandas/Made-With-ML](https://github.com/GokuMohandas/Made-With-ML)
- NN-deeplearning [https://zh.d2l.ai/](https://zh.d2l.ai/)
- Math & Python & ML [https://github.com/Visualize-ML](https://github.com/Visualize-ML)
- AI Papers w/ code [https://github.com/labmlai/annotated_deep_learning_paper_implementations](https://github.com/labmlai/annotated_deep_learning_paper_implementations
- Rag From Stratch by langchain: [https://github.com/langchain-ai/rag-from-scratch](https://github.com/langchain-ai/rag-from-scratch)
- Qwen Docs: [https://qwen.readthedocs.io/zh-cn/latest/index.html#](https://qwen.readthedocs.io/zh-cn/latest/index.html#)
- the bitter lesson: [https://cloud.tencent.com/developer/article/2119875](https://cloud.tencent.com/developer/article/2119875)
- [datawhalechina/llm-cookbook: 面向开发者的 LLM 入门教程，吴恩达大模型系列课程中文版 (github.com)](https://github.com/datawhalechina/llm-cookbook)
- langchain master class: [hw_dungeonrooms4q_h_en_115 (youtube.com)](https://www.youtube.com/watch?v=yF9kGESAi3M)

**Fundalmentals**

1. Python: [30 days of Python](https://github.com/Asabeneh/30-Days-Of-Python)；[AI Python for Beginners - DeepLearning.AI](https://www.deeplearning.ai/short-courses/ai-python-for-beginners/)
2. Math & Machine Learning:[Visualize-ML (Iris Series)](https://github.com/Visualize-ML)
3. Deep Learning: [D2l](https://courses.d2l.ai/zh-v2/)

### WhysAI

WhysAI由复旦大学几位在读博士发起，希望通过持续探索，来迈向卓越。Learn all we can，do the experiments，embrace the failures，then succeed。同时，欢迎关注公众号“WhysAI怀思智合”。

