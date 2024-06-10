# Assessing Coarse-to-Fine Deep Learning Models for Optic Disc and Cup Segmentation in Fundus Images

This repository contains an analysis of the use of Coarse-to-Fine models, as opposed to a single-stage model, for segmenting the optic disc and optic cup in fundus images. We also investigated whether the resulting segmentations could provide an accurate classification of glaucoma cases.

The vertical cup-to-disk ratio (vCDR) was calculated from the segmentations produced by the models. To compare our classifications with those of experts, we generated a dataset based on AIROGS images, consisting of 20 glaucoma and 20 non-glaucoma samples.

This work was submitted to SIPAIM 2022 under the title "Assessing Coarse-to-Fine Deep Learning Models for Optic Disc and Cup Segmentation in Fundus Images" to ensure reproducibility.

We present the segmentations obtained by each model and for each test dataset used: REFUGE, DRISHTI, RIM ONE V3, and ORIGA. Additionally, the dataset generated for comparison with experts is included, containing 40 samples from the AIROGS dataset (20 with glaucoma and 20 without glaucoma). The VCDR dataset is available in the file vCDR_dataframe.csv. This file contains the vCDR values provided by each expert, the average vCDR, the vCDR calculated from the TS-Model segmentation (OD → OD & OC), and the vCDR calculated from the SS-Model segmentation.

## Abstract

Automated optic disc (OD) and optic cup (OC) segmentation in fundus images is relevant to efficiently measure the vertical cup-to-disc ratio (vCDR), a biomarker commonly used in ophthalmology to determine the degree of glaucomatous optic neuropathy. In general this is solved using coarse-to-fine deep learning algorithms in which a first stage approximates the OD and a second one uses a crop of this area to predict OD/OC masks. While this approach is widely applied in the literature, there are no studies analyzing its real contribution to the results. In this paper we present a comprehensive analysis of different coarse-to-fine designs for OD/OC segmentation using 5 public databases, both from a standard segmentation perspective and for estimating the vCDR for glaucoma assessment. Our analysis shows that these algorithms not necessarily outperfom standard multi-class single-stage models, especially when these are learned from sufficiently large and diverse training sets. Furthermore, we noticed that the coarse stage achieves better OD segmentation results than the fine one, and that providing OD supervision to the second stage is essential to ensure accurate OC masks. Moreover, both the single-stage and two-stage models trained on a multi-dataset setting showed results close to other state-of-the-art alternatives in REFUGE and DRISHTI. Finally, we evaluated the models for vCDR prediction in comparison with six ophthalmologists on a subset of AIROGS images, to understand them in the context of inter-observer variability. We noticed that vCDR estimates recovered both from single-stage and coarse-to-fine models can obtain good glaucoma detection results even when they are not highly correlated with manual measurements from experts. 



## Citation

```
@inproceedings{moris2023assessing,
  title={Assessing coarse-to-fine deep learning models for optic disc and cup segmentation in fundus images},
  author={Moris, Eugenia and Dazeo, Nicol{\'a}s and de Rueda, Mar{\'\i}a Paula Albina and Filizzola, Francisco and Iannuzzo, Nicol{\'a}s and Nejamkin, Danila and Wignall, Kevin and Legu{\'\i}a, Mercedes and Larrabide, Ignacio and Orlando, Jos{\'e} Ignacio},
  booktitle={18th International Symposium on Medical Information Processing and Analysis},
  volume={12567},
  pages={232--241},
  year={2023},
  organization={SPIE}
}
```

## Contact

email: emoris@pladema.exa.unicen.edu.ar
