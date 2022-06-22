## CVPR 2022 Demo Track
___
### Paper
arXiv [link](https://arxiv.org/abs/2204.01715)

### Abstract
Most AI projects start with a Python notebook running on a single laptop; however, one usually needs to go through a mountain of pains to scale it to handle larger dataset (for both experimentation and production deployment). These usually entail many manual and error-prone
steps for the data scientists to fully take advantage of the available hardware resources (e.g., SIMD instructions, multi-processing, quantization, memory allocation optimization, data partitioning, distributed computing, etc.). To address this challenge, we have open sourced [BigDL
2.0](https://github.com/intel-analytics/BigDL/) under Apache 2.0 license (combining the original
BigDL and Analytics Zoo projects); using BigDL 2.0, users can simply build conventional Python notebooks on their laptops (with possible AutoML support), which can then be transparently accelerated on a single node (with up-to 9.6x speedup in our experiments), and seamlessly scaled out to a large cluster (across several hundreds servers in real-world use cases). BigDL 2.0 has already been adopted by many real-world users (such as Mastercard, Burger King, Inspur, etc.) in production.


## Demos
___
- **Online demo** at [Hugging Face Spaces](https://huggingface.co/spaces/CVPR/BigDL-Nano_inference) 

- [Notebooks](https://github.com/jason-dai/cvpr2022/tree/main/demos/FastFace) demostrating **accelerations for PyTorch Lightning** using BigDL-Nano

- *Yout may also refer to a collection of [BigDL notebooks](https://bigdl.readthedocs.io/en/latest/doc/UserGuide/notebooks.html) that can be directly opened and run in Colab*
