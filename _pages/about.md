---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>
我是山东师范大学的一名模拟IC设计方向的研二学生，指导老师是华庆([Qing Hua](http://www.physics.sdnu.edu.cn/info/1142/5730.htm))。研一时跟随导师的指导，做高压驱动芯片设计(1um)，熟悉设计软件和设计流程。同时自学拉扎维和桑森的书籍，沉淀模拟电路设计的基本功底。研二，开始由高压驱动芯片电路里的模块引申，例如电平位移和电压基准源电路，进行小模块电路创新设计。通过对相关方向论文的研究和总结，不断尝试，自主设计了带浮动衬底的电平位移电路(130nm)和带差分式输出的电压基准源电路(180nm)，另外还设计了三支路逻辑控制的电平位移电路(55nm)，有望发表**三篇质量中上的论文**。有读博继续深造的打算，要做就做最好。目前对IC电源方向（亚阈值低功耗）这一块积累较为深刻，对其它模拟IC方向抱有期待。

个人自评：有目标有规划，自驱力强，抗压能力强，能有效解决研究过程中碰到的问题。英语口语能力不错，能和外国人无障碍交流。学习能力强，硕士阶段很多研究方向都是由自己挖掘。希望能在未来博导的指引和教导下，在博士期间，至少发表一篇顶刊。如果有博导感兴趣，可以收藏我的简历[CV](https://github.com/zhouchch3/changchunzhou/blob/main/docs/CV.pdf)

<!--My research interest includes neural machine translation and computer vision. I have published more than 100 papers at the top international AI conferences with total <a href='https://scholar.google.com/citations?user=DhtAFkwAAAAJ'>google scholar citations <strong><span id='total_cit'>260000+</span></strong></a> (You can also use google scholar badge <a href='https://scholar.google.com/citations?user=DhtAFkwAAAAJ'><img src="https://img.shields.io/endpoint?url={{ url | url_encode }}&logo=Google%20Scholar&labelColor=f6f6f6&color=9cf&style=flat&label=citations"></a>).-->

# 📖 教育背景
- *2019.09 - 2023.06*, 土木工程, 成都大学（软科232）.

  大二决心学IC设计，自学电路基础、模拟电子技术基础、数字电子技术基础、信号与系统、半导体物理等多门课程
- *2023.09 - 至今*, 电子科学与技术, 山东师范大学（软科105）.

  自学《模拟CMOS集成电路设计》、《模拟集成电路设计精粹》等书籍

<!--# 🔥 News
- *2022.02*: &nbsp;🎉🎉 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 
- *2022.02*: &nbsp;🎉🎉 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. -->

# 🔥 模拟IC设计经历
- 2023.10~2024.6 ：**600V高压驱动芯片-1um**
  
  1、参与七通道驱动芯片设计：包括欠压保护电路，电平位移电路，高边驱动脉冲信号产生电路等。
  
  2、两通道驱动芯片：每个模块的电路设计和版图设计。电路能将5V的输入信号驱动600V高边输出和15V低边输出。最终半桥式驱动功率器件。对电压基准和电平位移等部分进行优化，达到了低延时的电路特性。
- 2024.04~2024.8：**带浮动衬底的电平位移电路-130nm**
  
  1、提出了一种浮动衬底技术，根据电路输出逻辑，反馈提供延时的大小可控的浮动电压，给电路输入直接驱动的正反逻辑器件提供衬底偏置。周期性地降低器件的阈值电压，同时降低电平位移时上下沿的延迟时间，小于2nS，最小输入电压降至0.17V。
  
  2、提出了一种电平位移基础结构，带有动态电流限制器件，同时降低了开关状态的静态功耗。最终EDP优于同类型平均水平一个数量级
- 2024.08~2024.12：**三支路逻辑控制电平位移-55nm**

  1、设计了三支路逻辑控制的电平位移，具有非常低的静态功耗，比同制程电路有更快的转换速度。
- 2024.04~2024.12：**CMOS电压基准源设计-180nm**

  1、提出了上厚下薄的伪共源共栅电流镜。提供的偏置电流精度非常高，输出电流偏差占比小于0.02%
  
  2、提出了两级自偏置的SDMT核心。提供两个参考电压。电压自偏置降低LS。
  
  3、提出了串联差分式输出结构。将两个参考电压进行差分，抵消PVT带来的偏差，并给予PVT补偿。通过差分和补偿，LS降低一半，PSRR全频域至少下降6dB，工艺角偏差小于10mV。温度偏差下降至1mV以内。
  
  4、提出关键极点偏移技术。PSRR极值下降了20%。通过极点叠加加速PSRR衰减，高频PSRR下降了7dB。
  
  5、提出了双输入启动电路。与单输入启动电路相比，静态功耗下降了三个数量级。

# 📝 成果转换

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">TCAS-II 2025（在投）</div><img src='images/图三.jpg' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">


**<u>Qun Zhou</u>**, Kang Zeng, Weiwei Yue and Qing Hua, Member, IEEE

*IEEE Transactions on Circuits and Systems II: Express Briefs (**TCAS-II**)*

<details>
<summary>Abstract</summary>
This brief presents an ultra-fast voltage level shifter (VLS) with a wide voltage conversion range. The proposed VLS achieves low symmetric propagation delay while operating in the subthreshold voltage, utilizing a newly introduced floating bias technique (FBT). By integrating a novel dynamic current limiter structure with a split inverter and pull-down devices, both the low-to-high and high-to-low delays are largely reduced. The  design of the proposed VLS is divided into two sections: the basic version and the enhanced version, which incorporates the FBT. Using a standard 130nm CMOS technology, the basic version demonstrates low propagation delay and high energy efficiency. Post-layout simulations, taking into account process, voltage, and temperature (PVT) variations, have been performed. With the implementation of the FBT, the delay is reduced to 2.09ns, dynamic power consumption is lowered to 27.3fJ, the minimum supply voltage is 0.17V, and the static power consumption is 9.7nW for the enhanced version.

</details>

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">TCAS-I 2025（在测）</div><img src='images/TCAS-II.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[Adjustable Multi-Stream Block-Wise Farthest Point Sampling Acceleration in Point Cloud Analysis](https://ieeexplore.ieee.org/document/10430381)

**<u>C. Zhou</u>**\*, Y. Fu*, Y. Ma, E. Han, Y. He, and H. Jiao

*IEEE Transactions on Circuits and Systems II: Express Briefs (**TCAS-II**)*


<details>
<summary>Abstract</summary>
Point cloud is increasingly used in a variety of applications. Farthest Point Sampling (FPS) is typically employed for down-sampling to reduce the size of point cloud and enhance the representational capability by preserving contour points in point cloud analysis. However, due to low parallelism and high computational complexity, high energy consumption and long latency are caused, which becomes a bottleneck of hardware acceleration. In this brief, we propose an adjustable multi-stream block-wise FPS, adjusted by four configurable parameters, according to hardware and accuracy requirements. A unified hardware architecture is designed to implement the adjustable multi-stream block-wise FPS. Furthermore, we present a rapid searching algorithm to select the optimal configuration of the four parameters. Designed in an industrial 28-nm CMOS technology, the proposed hardware architecture achieves a latency of 0.005 ms and a frame energy consumption of 0.09 µJ/frame for 1 k input points at 200 MHz and 0.9 V supply voltage. Compared to the state of the art, the proposed hardware architecture reduces the latency by up to 84.38%, saves the energy by up to 76.19%, and improves the network accuracy by up to 1.05%.

</details>

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ICCAD 2023</div><img src='images/ICCAD.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[An Energy-Efficient 3D Point Cloud Neural Network Accelerator With Efficient Filter Pruning, MLP Fusion, and Dual-Stream Sampling](https://ieeexplore.ieee.org/document/10323704)

**<u>C. Zhou</u>**, Y. Fu, M. Liu, S. Qiu, G. Li, Y. He, and H. Jiao.

*IEEE/ACM International Conference On Computer Aided Design (**ICCAD**)*


<details>
<summary>Abstract</summary>
Three-dimensional (3D) point cloud has been employed in a wide range of applications recently. As a powerful weapon for point cloud analysis, point-based point cloud neural networks (PNNs) have demonstrated superior performance with less computation complexity and parameters, compared to sparse 3D convolution-based networks and graph-based convolutional neural networks. However, point-based PNNs still suffer from high computational redundancy, large off-chip memory access, and low parallelism in hardware implementation, thereby hindering the applications on edge devices. In this paper, to address these challenges, an energy-efficient 3D point cloud neural network accelerator is proposed for on-chip edge computing. An efficient filter pruning scheme is used to skip the redundant convolution of pruned filters and zero-value feature channels. A block-wise multi-layer perceptron (MLP) fusion method is proposed to increase the on-chip reuse of features, thereby reducing off-chip memory access. A dual-stream blocking technique is proposed for higher parallelism while maintaining inference accuracy. Implemented in an industrial 28-nm CMOS technology, the proposed accelerator achieves an effective energy efficiency of 12.65 TOPS/W and 0.13 mJ/frame energy consumption for PointNeXt-S at 100 MHz, 0.9 V supply voltage, and 8-bit data width. Compared to the state-of-the-art point cloud neural network accelerators, the proposed accelerator enhances the energy efficiency by up to 66.6× and reduces the energy consumption per frame by up to 70.2×. 

</details>

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">IOT Journal 2023</div><img src='images/IOTJ.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[Sagitta: An Energy-Efficient Sparse 3D-CNN Accelerator for Real-Time 3D Understanding.](https://ieeexplore.ieee.org/abstract/document/10224248/)

**<u>C. Zhou</u>**, M. Liu, S. Qiu, X. Cao, Y. Fu, Y. He, and H. Jiao.

*IEEE Internet of Things Journal (**IOT Journal**)*


<details>
<summary>Abstract</summary>
Three-dimensional (3D) understanding or inference has received increasing attention, where 3D convolutional neural networks (3D-CNNs) have demonstrated superior performance compared to two-dimensional CNNs (2D-CNNs), since 3D-CNNs learn features from all three dimensions. However, 3D-CNNs suffer from intensive computation and data movement. In this paper, Sagitta, an energy-efficient low-latency on-chip 3D-CNN accelerator, is proposed for edge devices. Locality and small differential value dropout are leveraged to increase the sparsity of activations. A full-zero-skipping convolutional microarchitecture is proposed to fully utilize the sparsity of weights and activations. A hierarchical load-balancing scheme is also introduced to increase the hardware utilization. Specialized architecture and computation flow are proposed to enhance the effectiveness of the proposed techniques. Fabricated in a 55-nm CMOS technology, Sagitta achieves 3.8 TOPS/W for C3D at a latency of 0.1 s and 4.5 TOPS/W for 3D U-Net at a latency of 0.9 s at 100 MHz and 0.91 V supply voltage. Compared to the state-of-the-art 3D-CNN and 2D-CNN accelerators, Sagitta enhances the energy efficiency by up to 379.6× and 11×, respectively.

</details>

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">DAC 2021</div><img src='images/DAC.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[An Energy-Efficient Low-Latency 3D-CNN Accelerator Leveraging Temporal Locality, Full Zero-Skipping, and Hierarchical Load Balance](https://ieeexplore.ieee.org/document/9586299)

**<u>C. Zhou</u>**, M. Liu, S. Qiu, Y. He, and H. Jiao.

*IEEE/ACM Design Automation Conference (**DAC**)*


<details>
<summary>Abstract</summary>
Three-dimensional convolutional neural network (3D-CNN) has demonstrated outstanding classification performance in video recognition compared to two-dimensional CNN (2D-CNN), since 3D-CNN not only learns the spatial features of each frame, but also learns the temporal features across all frames. However, 3D-CNN suffers from intensive computation and data movement. To solve these issues, an energy-efficient low-latency 3D-CNN accelerator is proposed. Temporal locality and small differential value dropout are used to increase the sparsity of activation. Furthermore, to fully utilize the sparsity of weight and activation, a full zero-skipping convolutional microarchitecture is proposed. A hierarchical load-balancing scheme is also introduced to improve resource utilization. With the proposed techniques, a 3D-CNN accelerator is designed in a 55-nm low-power CMOS technology, bringing in up to 9.89x speedup compared to the baseline implementation. Benchmarked with C3D, the proposed accelerator achieves an energy efficiency of 4.66 TOPS/W at 100 MHz and 1.08 V supply voltage.

</details>

</div>
</div>



<div class='paper-box'><div class='paper-box-image'><div><div class="badge">TIM 2025</div><img src='images/TIM25_2StageEEG.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

A Two-Stage Prediction + Detection Framework for Real-Time Epileptic Seizure Monitoring

S. Qiu, W. Wang, **<u>C. Zhou</u>**, X. Song, J. Yang, and H. Jiao

*IEEE Transactions on Instrumentation and Measurement  (**TIM**)*


<details>
<summary>Abstract</summary>
The monitoring of epilepsy patients in non-hospital environment is highly desirable, where ultra-low power wearable devices are essential in such a system. The state-of-the-art epileptic seizure detection algorithms targeting such devices cannot achieve high sensitivity, short detection latency, low false alarm rate (FAR), as well as lightweight computing simultaneously. In this paper, we propose a two-stage prediction + detection deep neural network model, PDNet, for real-time epileptic seizure monitoring. The proposed two-stage PDNet model consists of a lightweight seizure predictor and a high-precision seizure detector. Only when the first-stage seizure predictor forecasts an impending seizure, the second-stage seizure detector is activated to precisely and rapidly classify the seizure states, thereby significantly suppressing the amount of computations. A semi-supervised learning strategy is employed to enhance the decision boundary of the seizure predictor, which is used for EEG pre-processing instead of pure prediction. Soft labels are adopted to enable the seizure detector to precisely classify the seizure states. The proposed PDNet is evaluated using the CHB-MIT scalp EEG database. When running the proposed prediction and detection models together for seizure detection purpose, the PDNet achieves 99.0% sensitivity, 0.54/h FAR, and 3.45-second detection latency with 3.03M multiply–accumulate (MAC) operations, which are competitive compared to the state of the art in terms of sensitivity, detection latency, FAR, and computation complexity. Furthermore, the fine-grained information such as the occurrence process of seizures demonstrated by soft labels can help the caregivers or clinicians to come up with targeted healthcare and clinical treatments.

</details>

</div>
</div>




<div class='paper-box'><div class='paper-box-image'><div><div class="badge">Symp. VLSI 2025</div><img src='images/VLSI25_PANDA.jpg' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

PANDA: A 3.178 TOPS/W Reconfigurable Seizure Prediction ANd Detection Neural Network Accelerator for Epilepsy Monitoring

S. Qiu, X. Song, X. Song, **<u>C. Zhou</u>**, X. Song, J. Yang, W. Wang, Y. Yang, and H. Jiao

*IEEE Symposium on VLSI Technology and Circuits (**Symp. VLSI**)*


<details>
<summary>Abstract</summary>
PANDA, a reconfigurable seizure prediction and detection neural network accelerator, is presented. A lightweight twostage seizure monitoring framework with temporal neural
network splitting is proposed to be deployed on PANDA. Channel first-output stationary dataflow with zero activation skipping and weight cache with statistical information are employed for higher energy efficiency. A flexible instruction set is defined to make PANDA highly configurable. For seizure monitoring, PANDA achieves up to 99% sensitivity, 0.43/h false alarm rate (FAR), and 3.178 TOPS/W energy efficiency.

</details>

</div>
</div>




<div class='paper-box'><div class='paper-box-image'><div><div class="badge">TBioCAS 2025</div><img src='images/EEG_TBioCAS.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[An Energy-Efficient Configurable 1-D CNN-Based Multi-Lead ECG Classification Coprocessor for Wearable Cardiac Monitoring Devices](https://ieeexplore.ieee.org/abstract/document/10844856)

C. Zhang, Z. Huang, **<u>C. Zhou</u>**, A. Qie, and X. Wang

*IEEE Transactions on Biomedical Circuits and Systems (**TBioCAS**)*


<details>
<summary>Abstract</summary>
Many electrocardiogram (ECG) processors have been widely used for cardiac monitoring. However, most of them have relatively low energy efficiency, and lack configurability in classification leads number and inference algorithm models. A multi-lead ECG coprocessor is proposed in this paper, which can perform efficient ECG anomaly detection. In order to achieve high sensitivity and positive precision of R-peak detection, a method based on zero-crossing slope adaptive threshold comparison is proposed. Also, a one-dimensional convolutional neural network (1-D CNN) based classification engine with reconfigurable processing elements (PEs) is designed, good energy efficiency is achieved by combining filter level parallelism and output channel parallelism within the PE chains with register level data reuse strategy. To improve configurability, a single instruction multiple data (SIMD) based central controller is adopted, which facilitates ECG classification with configurable number of leads and updatable inference models. The proposed ECG coprocessor is fabricated using 55 nm CMOS technology, supporting classification with an accuracy of over 98%. The test results indicate that the chip consumes 62.2 nJ at 100 MHz, which is lower than most recent works. The energy efficiency reaches 397.1 GOPS/W, achieving an improvement of over 40% compared to the reported ECG processors using CNN models. The comparison results show that this design has advantages in energy overhead and configurability.

</details>

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ISCAS 2024</div><img src='images/ISCAS.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[An Energy-Efficient Configurable Coprocessor Based on 1-D CNN for ECG Anomaly Detection](https://ieeexplore.ieee.org/abstract/document/10557838)

C. Zhang, Z. Huang, Q. Cheng, **<u>C. Zhou</u>**, and X. Wang

*IEEE International Symposium on Circuits and Systems (**ISCAS**)*


<details>
<summary>Abstract</summary>
Many healthcare devices have been widely used for electrocardiogram (ECG) monitoring. However, most of them have relatively low energy efficiency and lack flexibility. A novel ECG coprocessor is proposed in this paper, which can perform efficient ECG nomaly detection. In order to achieve high sensitivity and positive precision of R-peak detection, an algorithm based on Hilbert transform and adaptive threshold comparison is proposed. Also, a flexible one-dimensional convolutional neural network (1-D CNN) based classification engine is adopted, which can be configured with instructions to process various network models for ifferent applications. Good energy efficiency is achieved by combining filter level parallelism and output channel parallelism within the processing element (PE) array with data reuse strategy. A 1-D CNN for arrhythmia detection is proposed to validate the hardware performance. The proposed ECG coprocessor is implemented using 55 nm CMOS technology, occupying an area of 1.39 mm2. At a clock frequency of 100MHz, the energy efficiency is 215.6 nJ/classification. The comparison results show that this design has advantages in energy overhead and detection performance.

</details>

</div>
</div>



<div class='paper-box'><div class='paper-box-image'><div><div class="badge">TCSVT 2024</div><img src='images/TCAS-I.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[SoftAct: A High-Precision Softmax Architecture for Transformers with Nonlinear Functions Support](https://ieeexplore.ieee.org/document/10495359/)

Y. Fu, **<u>C. Zhou</u>**, T. Huang, E. Han, Y. He, and H. Jiao.

*IEEE Transactions on Circuits and Systems for Video Technology(**TCSVT**)*


<details>
<summary>Abstract</summary>
Transformer-based deep learning networks are revolutionizing our society. The convolution and attention codesigned (CAC) Transformers have demonstrated superior performance compared to the conventional Transformer-based networks. However, CAC Transformer networks contain various nonlinear functions, such as softmax and complex activation functions, which require high precision hardware design yet typically with significant cost in area and power consumption. To address these challenges, SoftAct, a compact and high-precision algorithm-hardware co-designed architecture, is proposed to implement both softmax and nonlinear activation functions in CAC Transformer accelerators. An improved softmax algorithm with penalties is proposed to maintain precision in hardware. A stage-wise full zero detection method is developed to skip redundant computation in softmax. A compact and reconfigurable architecture with a symmetrically designed linear fitting module is proposed to achieve nonlinear functions. The SoftAct architecture is designed in an industrial 28-nm CMOS technology with the MobileViT-xxs network as the benchmark. Compared with the state of the art, SoftAct achieves up to 35.14% network accuracy improvement, 10× maximum frequency, and 809× overall efficiency.

</details>

</div>
</div>




<div class='paper-box'><div class='paper-box-image'><div><div class="badge">TCSVT 2023</div><img src='images/TCSVT.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[CNN Accelerator at the Edge with Adaptive Zero Skipping and Sparsity-Driven Data Flow](https://ieeexplore.ieee.org/abstract/document/10122694/)

M. Liu, **<u>C. Zhou</u>**, S. Qiu, Y. He, and H. Jiao.

*IEEE Transactions on Circuits and Systems for Video Technology(**TCSVT**)*


<details>
<summary>Abstract</summary>
An energy-efficient convolutional neural network (CNN) accelerator is proposed for low-power inference on edge devices. An adaptive zero skipping technique is proposed to dynamically skip the zeros in either activations or weights, depending on which has the higher sparsity. The characteristic of non-zero data aggregation is explored to enhance the effectiveness of adaptive zero skipping in performance boosting. To mitigate the load imbalance issue after zero skipping, a sparsity-driven data flow and low-complexity dynamic task allocation are employed for different convolution layers. Facilitated further by a two-stage distiller, the proposed accelerator achieves 5.42×, 3.41×, and 3.42× performance boosting for VGG16, AlexNet, and Mobilenet-v1, respectively, compared to the baseline. Implemented in a 55-nm low power CMOS technology, the proposed accelerator achieves an effective energy efficiency of 2.41 TOPS/W, 2.35 TOPS/W, and 0.64 TOPS/W for VGG16, AlexNet, and Mobilenet-v1, respectively, at 100 MHz and 1.08 V supply voltage.

</details>

</div>
</div>


# 🍀 Tape Out

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">GenAI</div><img src='images/DiffusionChip.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

A energy-efficient diffusion chip for real-time and high-resolution images/videos generation at the edge.

12/2025 (Expected), Project Leader

*Fabricated in TSMC 16-nm FinFET technology with an expected area of 2 mm×4 mm*

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">HLS Chip</div><img src='images/HLSChip.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

A high-level synthesis based chip for CNN/Transformer architectures in general CV/NLP applications.

06/2025 (Expected), Collaboration

*Fabricated in TSMC 16-nm FinFET technology with an expected area of 1 mm×1 mm*

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">Transformer</div><img src='images/bit_variable_imc.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

A bit-variable in-memory computing chip for accelerating transformers at the edge.

06/2025 (Expected), Collaboration

*Fabricated in TSMC 40-nm technology with an expected area of 1 mm×1 mm*

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">Transformer</div><img src='images/nebula_v2_chip.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

An energy-efficient acceleration chip supporting transformer-based networks.

04/2025 (Expected), Project Leader

*Fabricated in TSMC 28-nm HPC technology with an expected area of 2 mm×3 mm*

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">Point Cloud</div><img src='images/28nm.jpg' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

An energy-efficient pipelined and configurable 3D point cloud-based neural network accelerator.

08/2023, Project Leader

*Fabricated in TSMC 28-nm HPC technology with an area of 2.0 mm×1.5 mm*

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">3D-CNN</div><img src='images/55nm_micrograph.jpg' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

A 4.5 TOPS/W sparse 3D-CNN accelerator for real-time 3D understanding

08/2020, Project Leader

*Fabricated in UMC 55-nm low-power CMOS technology with an area of 4.2 mm×3.6 mm*

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">1D-CNN</div><img src='images/1DCNN_Chips.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

1D-CNN accelerators for medical analysis

06/2024, Collaboration

*Fabricated in UMC 55-nm and TSMC 65-nm low-power CMOS technology*

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">2D-CNN</div><img src='images/LIU_28_Chip.jpg' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

A 2.4 TOPS/W CNN accelerator with adaptive zero skipping and sparsity-driven dataflow

06/2022, Collaboration

*Fabricated in TSMC 28-nm HPC technology with an area of 2.0 mm×1.35 mm*

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">2D-CNN</div><img src='images/LIU_55_Chip.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

A 2.0 TOPS/W CNN accelerator skipping invalid activations

10/2019, Collaboration

*Fabricated in UMC 55-nm low-power CMOS technology with an area of 3.4 mm×2.3 mm*

</div>
</div>




# 💻 Skills
- Flow: IC Front-End, Logic Synthesis, FPGA, Neural Network Training
- Tools: Cadence, Vivado, PyTorch, TensorFlow 
- Language: Verilog, SystemVerilog, Python, C, Shell, Makefile

# 💬 About Me
- I am an Easy Going and Self-Motivated Person. Feel Free to Reach out Anytime!
- Interests and Hobbies: Fitness, Taekwondo(Black Belt), and Table Tennis.


<!-- [**Project**](https://scholar.google.com/citations?view_op=view_citation&hl=zh-CN&user=DhtAFkwAAAAJ&citation_for_view=DhtAFkwAAAAJ:ALROH1vI_8AC) <strong><span class='show_paper_citations' data='DhtAFkwAAAAJ:ALROH1vI_8AC'></span></strong>
- Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 
</div>
</div>

- [Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet](https://github.com), A, B, C, **CVPR 2020**

# 🎖 Honors and Awards
- *2021.10* Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 
- *2021.09* Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 


# 💬 Invited Talks
- *2021.06*, Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 
- *2021.03*, Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet.  \| [\[video\]](https://github.com/)

# 💻 Internships
- *2019.05 - 2020.02*, [Lorem](https://github.com/), China. -->
