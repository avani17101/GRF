# GRF: Learning a General Radiance Field for 3D Scene Representation and Rendering
[Alex Trevithick](https://alextrevithick.github.io/), [Bo Yang](https://yang7879.github.io/), [arXiv:2010.04595](https://arxiv.org/abs/2010.04595), 2020

\[[Paper](https://arxiv.org/abs/2010.04595)\] \[Code (coming soon)\] \[[Video (Download for full 1008 by 756 resolution)](https://drive.google.com/file/d/1H2FNeAsKoQqCsO0n7PiA1HcT1ingnwJd/view?usp=sharing)\]

## (1) Qualitative Results on the Real-world Dataset
![](https://github.com/alextrevithick/GRF/blob/main/gifs/leaves.gif) |  ![](https://github.com/alextrevithick/GRF/blob/main/gifs/orchids.gif) | ![](https://github.com/alextrevithick/GRF/blob/main/gifs/fortress.gif) |  ![](https://github.com/alextrevithick/GRF/blob/main/gifs/trex.gif)
:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:
![](https://github.com/alextrevithick/GRF/blob/main/gifs/room.gif) |  ![](https://github.com/alextrevithick/GRF/blob/main/gifs/horns.gif) | ![](https://github.com/alextrevithick/GRF/blob/main/gifs/fern.gif) |  ![](https://github.com/alextrevithick/GRF/blob/main/gifs/flower.gif)

## (2) Qualitative Results on the Synthetic-NeRF Dataset
![](https://github.com/alextrevithick/GRF/blob/main/figs/qual_comp_real.png)

## (3) Qualitative Results on the ShapeNetv2 Dataset
<p align="center">
  <img src="https://github.com/alextrevithick/GRF/blob/main/gifs/car.gif" />
</p>    
<p align="center">
  <img src="https://github.com/alextrevithick/GRF/blob/main/gifs/chair.gif" />
</p>    

## (4) Overview of GRF
GRF is a powerful implicit neural function that can represent and render arbitrarily complex 3D scenes in a single network only from 2D observations. GRF takes a set of posed 2D images as input, constructs an internal representation for each 3D point of the scene, and renders the corresponding appearance and geometry of any 3D point viewing from an arbitrary angle. The key to our approach is to explicitly integrate the principle of multi-view geometry to obtain features representative of an entire ray from a given viewpoint. Thus, in a single forward pass to render a scene from a novel view, GRF takes some views of that scene as input, computes per-pixel pose-aware features for each ray from the given viewpoints through the image plane at that pixel, and then uses those features to predict the volumetric density and rgb values of points in 3D space. Volumetric rendering is then applied.
<p align="center">
  <img src="https://github.com/alextrevithick/GRF/blob/main/figs/fig_GRF.png" width="40%" />
</p>          

## (5) Quantative Results on the Real-world Dataset
![](https://github.com/alextrevithick/GRF/blob/main/figs/fig_results_LLFF.png)

## (6) Quantative Results the Synthetic-NeRF Dataset
![](https://github.com/alextrevithick/GRF/blob/main/figs/fig_results_Syn.png)

## (7) Quantative Results the ShapeNetv2 Dataset
![](https://github.com/alextrevithick/GRF/blob/main/figs/fig_results_shapenet.png)

### Citation
If you find our work useful in your research, please consider citing:

    @inproceedings{grf2020,
      title={GRF: Learning a General Radiance Field for 3D Scene Representation and Rendering},
      author={Trevithick, Alex and Yang, Bo},
      booktitle={arXiv:2010.04595},
      year={2020}
    }
