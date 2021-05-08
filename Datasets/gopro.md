# [Publications](../publications) | [Datasets](datasets) | [CV](../cv.pdf)
___

## GOPRO_Large dataset

GOPRO_Large dataset is proposed for dynamic scene deblurring.
Training and Test set are publicly available.

### <font color="FireBrick">Google Drive</font>

* [GOPRO_Large](https://drive.google.com/file/d/1y4wvPdOG3mojpFCHTqLgriexhbjoWVkK/view?usp=sharing): Blurry and sharp image pairs. Blurry images includes both gamma corrected and not corrected (linear CRF) versions.
* [GOPRO_Large_all](https://drive.google.com/file/d/1rJTmM9_mLCNzBUUhYIGldBYgup279E_f/view?usp=sharing): All the sharp images used to generate blurry images. You can generate new blurry images by accumulating differing number of sharp frames.

### <font color="FireBrick">SNU CVLab Server</font>

* [GOPRO_Large](http://data.cv.snu.ac.kr:8008/webdav/dataset/GOPRO/GOPRO_Large.zip): Blurry and sharp image pairs. Blurry images includes both gamma corrected and not corrected (linear CRF) versions.
* [GOPRO_Large_all](http://data.cv.snu.ac.kr:8008/webdav/dataset/GOPRO/GOPRO_Large_all.zip): All the sharp images used to generate blurry images. You can generate new blurry images by accumulating differing number of sharp frames.


## Reference

The GOPRO_Large dataset was proposed in CVPR 2017. If you find our dataset useful for your research, please consider citing our work:
* [paper](http://openaccess.thecvf.com/content_cvpr_2017/papers/Nah_Deep_Multi-Scale_Convolutional_CVPR_2017_paper.pdf)
* [supplementary](http://openaccess.thecvf.com/content_cvpr_2017/supplemental/Nah_Deep_Multi-Scale_Convolutional_2017_CVPR_supplemental.zip)
* [slides](https://drive.google.com/file/d/1sj7l2tGgJR-8wTyauvnSDGpiokjOzX_C/view?usp=sharing)
* [video](https://www.youtube.com/watch?v=L_YwOzRH28E&list=PLWTwxOOyqBYPh2xMPBMj-6L-CYRD48eAF)

```bibtex
@InProceedings{Nah_2017_CVPR,
  author = {Nah, Seungjun and Kim, Tae Hyun and Lee, Kyoung Mu},
  title = {Deep Multi-Scale Convolutional Neural Network for Dynamic Scene Deblurring},
  booktitle = {The IEEE Conference on Computer Vision and Pattern Recognition (CVPR)},
  month = {July},
  year = {2017}
}
```

### Github repository

The source code for training deblurring models are available:

* Torch7: [DeepDeblur_release](https://github.com/SeungjunNah/DeepDeblur_release)
* PyTorch: [DeepDeblur-PyTorch](https://github.com/SeungjunNah/DeepDeblur-PyTorch)
