# Assessing Coarse-to-Fine Deep Learning Models for Optic Disc and Cup Segmentation in Fundus Images

The use of Coarse-to-fine models, in contrast to a single-stage model, was analyzed in order to segment the optic disc and the optic cup on fundus images. At the same time, it was analyzed whether the segmentations obtained could give us an accurate classification of glaucoma cases. Consequently, if they could be used for the classification of glaucoma cases. The vertical cup to disk ratio (vCDR) was calculated from the segmentations obtained by the models. In order to compare our classification in relation to the vCDR calculated by the experts, a dataset based on AIROGS images was generated with 20 glaucoma images and 20 non-glaucoma samples.  The work were submitted to SIPAIM 2022 entitled "Assessing Coarse-to-Fine Deep Learning Models for Optic Disc and Cup Segmentation in Fundus Imagesa" in order to ensure reproducibility. 

The segmentations obtained by each model and on each test data used, which were REFUGE, DRISHTI, RIM ONE V3 and ORIGA, will be presented. At the same time, the dataset generated for the comparison with experts is also dated. It includes 40 samples from the AIROGS dataset (20 with glaucoma and 20 without glaucoma). The VCDR dataset is also contained in the file vCDR_dataframe.csv. It contains the vCDR given by each expert, the average of these vCDRs, the vCDR calculated from the TS-Model segmentation ($OD \rightarrow OD & OC$) and the vCDR calculated from the SS-Model segmentation. 

