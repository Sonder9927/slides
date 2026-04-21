---
theme: default
layout: cover
background: https://picsum.photos/id/1015/2000/1200  # 可换成海洋地震背景图（可选）
---

# OBS 海底地震仪互相关时频分析 Overview

**信号处理**  
时频分析与频散曲线提取  

**重点**：海水层 Scholte 波对短周期（<10 s）频散的影响  
（暂无实际结果，仅方法与思想概述）

---

# 1. 研究背景

- 背景噪声互相关（Ambient Noise Cross-Correlation）是提取经验格林函数的重要手段
- OBS（Ocean Bottom Seismometer）在海洋地震学中广泛应用，可记录海底噪声
- 与大陆台站相比，海洋环境存在显著的海水层，导致波场传播差异
- 本项目结合信号处理技术，对 OBS 互相关结果进行深入分析

<div class="flex justify-center items-center" style="height: 65%;">
  <img
    src="/images/msignal/obs-deploy.png"
    alt="OBS 海底地震仪部署示意图"
    style="max-width: 90%; max-height: 100%; object-fit: contain;"
  >
</div>

---

# 2. 科学问题

**核心问题**：
海水层的存在使 Scholte 波（界面波）在短周期（10 s 以下）占主导，导致 OBS 互相关频散曲线与大陆台站（主要 Rayleigh 波）显著不同。

- 科学意义：揭示海洋-大陆地壳结构差异
- 信号处理视角：短周期频散受水层影响更敏感，需特殊方法分离与分析
- 预期差异：大陆台站频散曲线平滑；OBS 在 <10 s 出现明显低速区或拐点

---

# 3. 信号分析流程

1. **数据预处理**：互相关计算、时域 stacking、谱白化（whitening）、带通滤波
2. **时频分析**：FTAN（频率-时间分析），生成时频谱
3. **频散曲线提取**：相/群速度频散测量
4. **对比分析**：OBS vs 大陆台站频散曲线
5. **物理机制解释**：Scholte 波影响 <10 s 频散

<div class="flex justify-center items-center" style="height: 65%;">
  <img
    src="/images/msignal/ftan.png"
    alt="时频分析与互相关示例"
    style="max-width: 90%; max-height: 100%; object-fit: contain;"
  >
</div>

---

# 4. 亮点与总结

- **亮点**：体现海水层 Scholte 波对短周期频散的独特影响
- 充分融合信号处理思想：互相关、时频变换、频散拾取、多站对比
- 预期成果：展示 OBS 与大陆台站频散曲线的差异（<10 s 段）
- 下一步：实际数据处理与结果验证

**感谢聆听**  
Q&A  
