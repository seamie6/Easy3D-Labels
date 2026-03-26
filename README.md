<div align="center">
  
# Easy3D-Labels: Supervising Semantic Occupancy Estimation with 3D Pseudo-Labels for Automotive Perception

<p align="center">
  <a href="https://scholar.google.com/citations?user=3fffnjYAAAAJ&hl=en"><strong>Seamie Hayes</strong></a><sup>1,2</sup>,
  <a href="https://scholar.google.com/citations?user=356ahmwAAAAJ&hl=en"><strong>Ganesh Sistu</strong></a><sup>1</sup>,
    <a href="https://scholar.google.com/citations?user=dDgm87sAAAAJ&hl=en"><strong>Tim Brophy</strong></a><sup>1</sup>,
  <a href="https://scholar.google.com/citations?user=aH6w8VcAAAAJ&hl=en"><strong>Ciaran Eising</strong></a><sup>1,2</sup>
</p>


<p align="center">
<sup>1</sup> D²iCE Research Centre, University of Limerick &nbsp;&nbsp; <sup>2</sup> Taighde Éireann – Research Ireland &nbsp;&nbsp
</p>

[![arXiv](https://img.shields.io/badge/arXiv-2509.26087-b31b1b)](https://arxiv.org/abs/2509.26087)
[![Mendeley](https://img.shields.io/badge/Mendeley-9scymfs7xv-orange)](https://data.mendeley.com/datasets/9scymfs7xv/1)
</div>

## Easy3D-Labels: 3D Pseudo-Label Construction
<img src="assets/labels.jpg" width="100%">

## EasyOcc Model
<img src="assets/easyocc.jpg" width="100%">

## Abstract
_In perception for automated vehicles, safety is critical not only for the driver but also for other agents in the scene, particularly vulnerable road users such as pedestrians and cyclists. Previous representation methods, such as Bird’s Eye View, collapse vertical information, leading to ambiguity in 3D object localisation and limiting accurate understanding of the environment for downstream tasks such as motion planning and scene forecasting. In contrast, semantic occupancy provides a full 3D representation of the surroundings, addressing these limitations. Furthermore, self-supervised semantic occupancy has seen increased attention in the automated vehicle domain. Unlike supervised methods that rely on manually annotated data, these approaches use 2D pseudo-labels, improving scalability by reducing the need for labour-intensive annotation. Consequently, such models employ techniques such as novel view synthesis, cross-view rendering, and depth estimation to allow for model supervision against the 2D labels. However, such approaches often incur high computational and memory costs during training, especially for novel view synthesis. To address these issues, we propose Easy3D-Labels, which are 3D pseudo-ground-truth labels generated using Grounded-SAM and Metric3Dv2, with temporal aggregation for densification, permitting supervision directly in 3D space. Easy3D-Labels can be readily integrated into existing models to provide model supervision, yielding substantial performance gains, with mIoU increasing by 45\% and RayIoU by 49\% when applied to OccNeRF on the Occ3D-nuScenes dataset. Additionally, we introduce EasyOcc, a streamlined model trained solely on these 3D pseudo-labels, avoiding the need for complex rendering strategies, and achieving 15.7 mIoU on Occ3D-nuScenes. Easy3D-Labels improve scene understanding by reducing object duplication and enhancing depth estimation accuracy, as reflected by improvements in the RayIoU metric. These findings highlight the importance of foundation models, temporal information, and 3D loss formulation in self-supervised learning for comprehensive scene understanding._

## Dataset
The dataset is publicly available on [Mendeley](https://data.mendeley.com/datasets/9scymfs7xv/1)

## Acknowledgement
This publication has emanated from research conducted with the financial support of Taighde Éireann – Research Ireland under Grant number 18/CRT/6049. For the purpose of Open Access, the author has applied a CC BY public copyright licence to any Author Accepted Manuscript version arising from this submission.

I would like to thank the authors of the following open-source projects:<br>
[GaussianOcc](https://github.com/GANWANSHUI/GaussianOcc)<br>
[OccNeRF](https://github.com/LinShan-Bin/OccNeRF)<br>
[SelfOcc](https://github.com/huang-yh/SelfOcc)<br>

## Citation
```
@misc{hayes2025easyocc3dpseudolabelsupervision,
      title={EasyOcc: 3D Pseudo-Label Supervision for Fully Self-Supervised Semantic Occupancy Prediction Models}, 
      author={Seamie Hayes and Ganesh Sistu and Ciarán Eising},
      year={2025},
      eprint={2509.26087},
      archivePrefix={arXiv},
      primaryClass={cs.CV},
      url={https://arxiv.org/abs/2509.26087}, 
}
```
