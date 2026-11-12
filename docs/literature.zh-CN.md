# 相关研究文献

以下是睡眠监测、PPG 和心率变异性的初始阅读清单。文献用于提供背景，不代表本开发平台已经达到论文中的性能。

## 睡眠监测与验证

### Wearable Sleep Technology in Clinical and Research Settings

- 作者：Massimiliano de Zambotti、Nicola Cellini、Aimée Goldstone、Ian M. Colrain、Fiona C. Baker
- 期刊：*Medicine & Science in Sports & Exercise*，2019，51(7)，1538-1557
- DOI：[10.1249/MSS.0000000000001947](https://doi.org/10.1249/MSS.0000000000001947)

该综述讨论消费级睡眠追踪器、验证要求，以及专有算法、固件变化和设备可靠性等影响因素。

## PPG 与加速度计睡眠分期

### Estimation of sleep stages in a healthy adult population from optical plethysmography and accelerometer signals

- 作者：Z. Beattie、Y. Oyang、A. Statan、A. Ghoreyshi、A. Pantelopoulos、A. Russell、C. Heneghan
- 期刊：*Physiological Measurement*，2017，38(11)，1968-1979
- DOI：[10.1088/1361-6579/aa9047](https://doi.org/10.1088/1361-6579/aa9047)

论文研究使用光学脉搏波和加速度信号估计睡眠阶段，与本项目的主要传感器组合直接相关。

## 心率变异性与机器学习

### Sleep stage classification from heart-rate variability using long short-term memory neural networks

- 作者：Mustafa Radha、Pedro Fonseca、Arnaud Moreau、Marco Ross、Andreas Cerny、Peter Anderer、Xi Long、Ronald M. Aarts
- 期刊：*Scientific Reports*，2019，9，14149
- DOI：[10.1038/s41598-019-49703-y](https://doi.org/10.1038/s41598-019-49703-y)

该工作展示使用 LSTM 从心率变异性进行睡眠阶段分类的方法，可作为特征分析参考。

## 阅读注意事项

- 文献性能依赖传感器位置、研究人群和参考评分方法。
- PPG 得到的搏动间期不能默认等同于 ECG 得到的间期。
- 报告睡眠阶段时，应同时说明验证方法、样本规模和局限。
- 本项目不能直接把论文性能当作自身验证结果。
