<!-- - XXXXXXX论文

- XXXXXXX论文

- XXXXXXX论文
 -->

<!-- - **HEncode: A Highly Modularized and Efficient FPGA QC-LDPC Encoder Using High Level Synthesis**
  - **杨嘉伟**, [其他作者]
  - *The 42nd IEEE International Conference on Computer Design (* **ICCD 2024, CCF-B** *), Accepted.*
  - 我作为 **第一作者**，负责设计并实现了一种近 Tbps 吞吐率的 QC-LDPC 编码器。

- **HeteroGNN: A Heterogeneous Stage Division Based GNN Training Framework to Maximize CPU-GPU Parallelism**
  - [其他作者], **杨嘉伟**
  - *IEEE International Conference on Multimedia and Expo (* **ICME 2025, CCF-B** *), Accepted.*
  - 我作为 **第三作者**，参与设计了数据依赖感知的阶段划分策略和自适应任务调度器。

- **eLDPC: An Elastic HLS-friendly LDPC-Decoder with Dynamical Scheduling**
  - [参与作者], **杨嘉伟**, [其他作者]
  - *投稿中*
  - 我作为 **参与者**，主要负责优化 HLS 在任务级调度中的表现。 -->

### 高性能GPU倒排索引与稀疏计算优化

独立研究项目 | 2025.04 - 至今

- **Sparse Bool GPU Kernel for IR System**（计划投稿SIGMOD）：为加速信息检索与推荐系统中的稀疏计算，设计并实现了一套高性能GPU倒排索引库。将倒排链根据元素值的高位进行分块 ，再依据块内元素密度从多种稀疏与稠密格式中选择最优压缩方式进行存储。与主流GPU稀疏计算库cuBool相比，该方案的稀疏计算性能提升约**79%**

###  面向CPU-GPU并行的GNN训练框架设计与优化 
<!-- Transformer 模型异构硬件推理加速 -->

开放合作研究课题 - 光明实验室 GNN优化加速 | 2025.01 - 至今

- [**HeteroGNN: A Heterogeneous Stage Division Based GNN Training Framework to Maximize CPU-GPU Parallelism**](https://whova.com/embedded/session/hlWY6K3rL7pHvG8Yd1TfjYJVgDEZvOuEPKWGmeuUbIQ%3D/4654604/?widget=primary)（ICME25'）：设计并实现了GNN训练框架HeteroGNN，提出了数据依赖感知的阶段划分策略，将训练过程从粗粒度的两个阶段细化为六个阶段，实现了阶段间的并行
- HeteroGNN还设计了细粒度的计算划分模式和自适应任务调度器，根据拓扑结构的特性，在CPU和GPU上合理地分配计算任务，有效提升了GPU的利用率 。实验结果表明，HeteroGNN相比于DGL和PyG，实现了**1.3**倍到**2.06**倍的端到端训练加速

### 国家重点研发项目：全息存储多级长效编码与数据通道
  
项目编号No. 2018YFA0701800 | 2022.09 - 2024.09

- [**HEncode: A Highly Modularized and Efficient FPGA QC-LDPC Encoder Using High Level Synthesis**](https://ieeexplore.ieee.org/document/10818010/)（ICCD24'，**第一作者**）: 使用C/C++以及优化高层次综合(HLS)，在FPGA上实现近Tbps级别吞吐率的QC-LDPC编码器，设计实现了3级并行和2级流水的编码计算操作，实现**5.89×**的单位硬件效率提升和**154.5×**的最高编码吞吐率提升，实现了**922.66Gbps**的编码效率

- **eLDPC: An Elastic HLS-friendly LDPC-Decoder with Dynamical Scheduling**(TCAD在投): 优化HLS在任务级调度中的表现，使用双缓冲区和重构输出缓冲优化译码器中译码单元运行时间不对齐的问题，综合吞吐率较SOTA提升**5×**


### 黑色素瘤致癌基因筛选

病毒学国家重点实验室 - 生信分析 数据分析员 | 2022.03 - 2022.05

- 利用支持向量机对测序数据初步验证，使用随机森林算法，LASSO回归和递归特征消除算法对进行特征提取并最终确定**8个**潜在的黑色素瘤的**相关基因**，其中部分已被证实存在相关性，也存在尚未背研究的基因，提示后续的实验开展方向