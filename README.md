# StyleMaster
<div align="center">

[![CVPR'25](https://img.shields.io/badge/arXiv%20paper-2410.10511-b31b1b)](https://arxiv.org/abs/)&nbsp;
[![project page](https://img.shields.io/badge/Project%20page-StyleMaster-pink)](https://zixuan-ye.github.io/stylemaster.github.io/)&nbsp;

</div>


**[StyleMaster: Stylize Your Video with Artistic Generation and Translation](https://arxiv.org/abs/)**

[video](https://github.com/zixuan-ye/stylemaster/blob/main/assets/teaser.mp4)


[Zixuan Ye](https://zixuan-ye.github.io/)<sup>1 &dagger;</sup>, [Huijuan Huang](https://openreview.net/profile?id=~Huijuan_Huang1)<sup>2&#9993;</sup>, [Xintao Wang](https://xinntao.github.io/)<sup>2</sup>, [Pengfei Wan](https://scholar.google.com/citations?user=P6MraaYAAAAJ&hl=en)<sup>2</sup>, [Di Zhang](https://openreview.net/profile?id=~Di_ZHANG3)<sup>2</sup>, [Wenhan Luo](https://whluo.github.io/)<sup>1&#9993;</sup>

1 Hong Kong University of Science and Technology  
2 Kuaishou Technology  
† Intern at KwaiVGI, Kuaishou Technology  
✉ Corresponding Author

## TODO
- [ ] Implementation on videotuna
- [ ] Code and weight of style extraction module
- [x] Illusion dataset generation

## Update
- [2025.2] StyleMaster has been accepted by CVPR2025!
- [2024.10] [arXiv](https://arxiv.org/abs/) preprint is available.

## Introduction

Welcome to **StyleMaster**! StyleMaster focuses on style control, i.e., generating or translating a video to match the style of a given reference image. StyleMaster preserves local textures and enhance global style representations. Additionally, a motion adapter and gray tile ControlNet are employed to enhance motion quality and provide precise content guidance.

## Features

- **Local Patch Selection**: Overcomes content leakage in style transfer by selecting patches with less similarity to text prompts.
- **Global Style Extraction**: Uses a projection module after CLIP supervised by illusion datasets.
- **Motion Adapter**: Enhances motion quality during inference and helps to enhance the style extent.
- **Gray Tile ControlNet**: Provides accessible yet precise content guidance for video style transfer.
- **High-Quality Video Generation**: Generates videos with high style similarity to the reference image and achieves ideal translation results.

## Illusion Dataset Generation
Please refer to [visual_anagrams/readme.md](visual_anagrams/readme.md) for details.


## Citation

```bibtex
@article{ye2024stylemaster,
  title={StyleMaster: Stylize Your Video with Artistic Generation and Translation},
  author={Ye, Zixuan and Huang, Huijuan and Wang, Xintao and Wan, Pengfei and Zhang, Di and Luo, Wenhan},
  journal={arXiv preprint arXiv:},
  year={2024}
}