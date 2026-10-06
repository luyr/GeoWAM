# GeoWAM: Visual Geometry World Action Models for Autonomous Driving

[**Project Page**](https://yiren-lu.com/project_pages/GeoWAM/) | [**arXiv**](https://arxiv.org/abs/2608.23486)

---

## 🚧 Code Coming Soon

The code and models for GeoWAM will be released here. Stay tuned!

GeoWAM is a visual geometry world action model for autonomous driving that treats 3D geometry, rather than pixels, as the state space of the world. Instead of generating future images, GeoWAM is pretrained to forecast future scene geometry as dense point maps, and a geometry-conditioned action head infers the ego trajectory consistent with the predicted scene evolution.

Because geometry pretraining learns directly from raw multiview image sequences, it scales with unlabeled driving data and needs no trajectory annotations. Scaling pretraining from 0 to 832 hours of PhysicalAI driving data raises the NAVSIM `navhard` EPDMS by 8.2% to 39.6 and halves the zero-shot collision rate on nuScenes to 0.12%. These gains come with no added model capacity, no extra trajectory supervision, and no PDMS-based supervision.

<p align="center">
  <img src="./assets/framework.webp" alt="GeoWAM architecture" width="100%"/>
</p>

## Citation

```bibtex
@article{lu2026geowam,
  title={GeoWAM: Visual Geometry World Action Models for Autonomous Driving},
  author={Lu, Yiren and Ye, Xin and Liu, Jiaming and Jacobson, Philip and Yao, Jin and Chen, Yi-chung and Merino, Liam and Kurra, Dhruva Dixith and Cai, Min and Lampo, Tom and others},
  journal={arXiv preprint arXiv:2608.23486},
  year={2026}
}
```
