# Quant-dLLM: Post-Training Extreme Low-Bit Quantization for Diffusion Large Language Models

Tianao Zhang, [Zhiteng Li](https://zhitengli.github.io), Xianglong Yan, [Haotong Qin](https://htqin.github.io/), Yong Guo, and [Yulun Zhang](http://yulunzhang.com/).

[[arXiv](https://arxiv.org/abs/2510.03274)] [models]

#### 🔥🔥🔥 News

- **2025-10-07:** This repo is released.


![](figs/overview_v2.pdf)
--- 

> **Abstract:** Diffusion large language models (dLLMs), which offer bidirectional context and flexible masked-denoising generation, are emerging as a compelling alternative to autoregressive (AR) LLMs. However, like AR LLMs, their model sizes continue to grow, motivating weight compression for deployment. Although post-training quantization (PTQ) is effective for AR LLMs, directly transferring it to dLLMs at 2-bit leads to unsatisfactory performance. To tackle these challenges, we propose Quant-dLLM, an ultra-low-bit PTQ framework tailored to dLLMs. Since masked-denoising activations in dLLMs differ from the fully visible signals assumed by standard PTQ methods, we introduce Masked Calibration Simulation (MCS) to align calibration with the timestep-dependent masking, which yields more reliable calibrations. Moreover, we propose a Data-aware Any-order Quantizer (DAQ) that learns ultra-low-bit weight representations via an optimization algorithm. It performs iterative approximation guided by our simulated calibration data. In addition, under a strict 2-bit budget, we introduce Adaptive Blockwise Mixed Precision (ABMP), a sensitivity-based precision allocation scheme that adaptively assigns bit width across channel groups. When restricted to 2-bit precision, Quant-dLLM consistently achieves higher accuracy than state-of-the-art (SOTA) AR-transfer PTQ methods on dLLMs. The code and models will be available at: https://github.com/ZTA2785/Quant-dLLM

---

## ⚒️ TODO

* [ ] Complete this repository

## 🔗 Contents

- [ ] Post-training quantization
- [ ] Models
- [x] [Results](#Results)
- [x] [Citation](#Citation)
- [x] [Acknowledgements](#Acknowledgements)

## Citation

If you find the code helpful in your research or work, please cite the following paper.

```
@article{zhang2025quantdllmposttrainingextremelowbit,
      title={Quant-dLLM: Post-Training Extreme Low-Bit Quantization for Diffusion Large Language Models}, 
      author={Tianao Zhang and Zhiteng Li and Xianglong Yan and Haotong Qin and Yong Guo and Yulun Zhang},
      year={2025},
      eprint={2510.03274},
      archivePrefix={arXiv},
      primaryClass={cs.LG},
      url={https://arxiv.org/abs/2510.03274}, 
}
```

## 💡 Acknowledgements

This work is released under the Apache 2.0 license.
