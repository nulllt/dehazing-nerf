# Dehazing-NeRF: Neural Radiance Fields from Hazy Images

## Abstract

The Neural Radiance Field (NeRF) technique shines among recent image processing approaches due to its superior capabilities in high-quality 3D scene reconstruction and novel view synthesis. However, image degradation caused by the scattering of atmospheric light and object light by particles in the atmosphere can significantly decrease the reconstruction quality when shooting scenes in hazy conditions. To tackle this challenge, we propose Dehazing-NeRF, a method designed to restore clear NeRF from hazy image inputs. Our approach simulates the physical imaging process of hazy images using an atmospheric scattering model. It simultaneously learns the scattering properties and a clean NeRF model to facilitate image dehazing and novel view synthesis. Different from previous approaches, Dehazing-NeRF is an unsupervised method with only hazy images as the input and also does not depend on manually crafted dehazing priors. By integrating the depth estimated from the NeRF 3D scene with the atmospheric scattering model, our proposed model overcomes the inherent challenges of single-image dehazing while maintaining geometric consistency. Additionally, we propose a multi-objective optimization strategy including soft margin consistency regularization, atmospheric consistency, and contrast discriminative loss. These components effectively mitigate the degradation of scene reconstruction quality caused by information loss during model training. Extensive experiments demonstrate that our method outperforms the simple combination of single-image dehazing and NeRF on both image dehazing and novel view image synthesis.



## BibTeX
If you find our work useful for your project, please consider citing the following paper.
```
@article{li2023dehazing,
  title={Dehazing-NeRF: neural radiance fields from hazy images},
  author={Li, Tian and Li, LU and Wang, Wei and Feng, Zhangchi},
  journal={arXiv preprint arXiv:2304.11448},
  year={2023}
  eprint={2311.17245},
  archivePrefix={arXiv},
  primaryClass={cs.CV} }
}
```
