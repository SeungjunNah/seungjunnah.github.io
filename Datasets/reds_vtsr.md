# [Publications](../publications) | [Datasets](datasets) | [CV](../cv.pdf)
___

## <font color="red">REDS_VTSR</font> dataset

We provide the **<font color="red">RE</font>**alistic and **<font color="red">D</font>**ynamic **<font color="red">S</font>**cenes dataset for **V**ideo **T**emporal **S**uper-**R**esolution (frame interpolation). Train and validation subsets are publicly available.
Downloads are available via Google Drive and Huggingface.

### <font color="FireBrick">Google Drive</font>

Type | Train | Validation | Test
-- | -- | -- | --
15fps | [train_15fps](https://drive.google.com/file/d/17iATapUjImmvE_NrX8kVlrLROiFJWO91/view?usp=sharing) | [val_15fps](https://drive.google.com/file/d/1HHVsk0o3wgMIf4FD6mMUyW0w7uawBrkQ/view?usp=sharing) | [test_15fps](https://drive.google.com/file/d/1AB7QwcpIPSaAEt01wkIejZaXTXlChs53/view?usp=sharing)
30fps | [train_30fps](https://drive.google.com/file/d/10fgQ2cOksfsntdwzSUlWuJcnKrvRCVww/view?usp=sharing) | [val_30fps](https://drive.google.com/file/d/1tyj-7YhMx7-E7x5Z8XV1bBVlOGF3bgTj/view?usp=sharing) | test_30fps
60fps | [train_60fps](https://drive.google.com/file/d/1jwImdo65ZU6HXALq9Xee5S56AcSqePif/view?usp=sharing) | [val_60fps](https://drive.google.com/file/d/1PKK1tgddL8uQ6LMehrAe8RViUYiXxTHj/view?usp=sharing) | test_60fps

### <font color="FireBrick">Huggingface</font>

Type | Train | Validation | Test
-- | -- | -- | --
15fps | [train_15fps](https://huggingface.co/datasets/snah/REDS_VTSR/resolve/main/train_15fps.zip) | [val_15fps](https://huggingface.co/datasets/snah/REDS_VTSR/resolve/main/val_15fps.zip) | [test_15fps](https://huggingface.co/datasets/snah/REDS_VTSR/resolve/main/test_15fps.zip)
30fps | [train_30fps](https://huggingface.co/datasets/snah/REDS_VTSR/resolve/main/train_30fps.zip) | [val_30fps](https://huggingface.co/datasets/snah/REDS_VTSR/resolve/main/val_30fps.zip) | test_30fps
60fps | [train_60fps](https://huggingface.co/datasets/snah/REDS_VTSR/resolve/main/train_60fps.zip) | [val_60fps](https://huggingface.co/datasets/snah/REDS_VTSR/resolve/main/val_60fps.zip) | test_60fps


## Updates

* We are planning to host an open-end public leaderboard site for the **<font color="red">REDS</font>** related challenges. 
We will provide evaluated PSNR and SSIM for the submitted test results.
Stay tuned for the updates!

## Reference

The **<font color="red">REDS_VTSR</font>** dataset was used in the AIM 2019 and AIM 2020 Challenges. If you find our dataset useful for your research, please consider citing our work:

* **<font color="red">REDS_VTSR</font>** dataset and the AIM 2019 Challenge [[paper](https://cv.snu.ac.kr/publication/conf/2019/aim2019_vtsr.pdf)] [[arXiv](https://arxiv.org/abs/2005.01233)] [[slides](https://drive.google.com/file/d/1Y9Se8LPlDUWuaVzEcFvzHlCpD6X4-gOO/view?usp=sharing)]

```bibtex
@InProceedings{Nah_2019_ICCV_Workshops_REDS_VTSR,
  author = {Nah, Seungjun and Son, Sanghyun and Timofte, Radu and Lee, Kyoung Mu},
  title = {AIM 2019 Challenge on Video Temporal Super-Resolution: Methods and Results},
  booktitle = {ICCV Workshops},
  month = {Oct},
  year = {2019}
}
```

* **<font color="red">REDS_VTSR</font>** AIM 2020 Challenge [[paper](https://cv.snu.ac.kr/publication/conf/2019/aim2020_vtsr.pdf)] [[arXiv](https://arxiv.org/abs/2009.12987)] [[slides](https://drive.google.com/file/d/1C4E21NlH2H2EoQ0TidNJmT1ruEOyac8M/view?usp=sharing)]

```bibtex
@InProceedings{Son_2020_ECCV_Workshops_VTSR,
  author = {Son, Sanghyun and Lee, Jaerin and Nah, Seungjun and Timofte, Radu and Lee, Kyoung Mu},
  title = {AIM 2020 Challenge on Video Temporal Super-Resolution},
  booktitle = {ECCV Workshops},
  month = {Aug},
  year = {2020}
}
```

## LICENSE

REDS_VTSR dataset is released under [CC BY 4.0 license](https://creativecommons.org/licenses/by/4.0/).
