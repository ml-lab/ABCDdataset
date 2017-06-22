# ABCD dataset

This material is a description of ABCD (AIST Building Change Detection) dataset.
This dataset is a new labeled dataset, specially geared toward constructing and evaluating damage detection systems to identify whether buildings have been washed-away by tsunami.


## Description
Each datum in this dataset is a pair of pre- and post-tsunami aerial image patches, and encompasses a target building at the center of the patch. These pairs were cropped from a hefty number of RGB aerial images taken before or after the Tohoku earthquake, with the original pixel resolution of 40 cm for pre-quake images and 12 cm for post-qukae images (actually, resampled to 40 cm).

The below shows eight samples from the dataset, where four pairs are shown for "washed-away" class (left column) and "surviving" class (right column), respectively. The class label annotated to each pair means whether or not a building at the center of the pre-tsunami patch got wahshed-away. 

![patches_](https://user-images.githubusercontent.com/13417696/27384118-b5539e1e-56c8-11e7-9c0c-7d06b899763f.png)


We prepared this set for three types of scale: fixed-scale, size-adaptive and resized. Fixed-scale patches have the same resolution of the original images (40 cm) and the patch size is 160 x 160 pixels. Size-adaptive patches 
The resulting ABCD dataset comprised 10,777 pairs for fixed-scale (4,253 washed-away) and 11,394 pairs for size-adaptive and resized (4,546 washed-away). 


Please see the following paper for further details, and cite the paper when publishing results that use this dataset:  
**Aito Fujita, Ken Sakurada, Tomoyuki Imaizumi, Riho Ito, Shuhei Hikosaka and Ryosuke Nakamura, "Damage Detection from Aerial Images
via Convolutional Neural Networks," IAPR International Conference on Machine Vision Applications (MVA), 2017.**


---

Aito Fujita  
National Institute of Advanced Industrial Science and Technology (AIST), Japan  
Email: fujita.713@aist.go.jp  

This dataset is based on results obtained from a project commissioned by the New Energy and Industrial Technology Development Organization (NEDO).
