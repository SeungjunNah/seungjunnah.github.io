# [Publications](../publications) | [Datasets](datasets) | [CV](../cv.pdf)

## <font color="red">REDS</font> dataset

We provide the **<font color="red">RE</font>**alistic and **<font color="red">D</font>**ynamic **<font color="red">S</font>**cenes dataset for video deblurring and super-resolution. Train and validation subsets are publicly available.
The dataset can be downloaded by running the below python code or by clicking the links.

[download_REDS.py](https://gist.github.com/SeungjunNah/b10d369b92840cb8dd2118dd4f41d643)

Type | Train | Validation | Test
-- | -- | -- | -- | --
Sharp | [train_sharp](https://drive.google.com/open?id=1YLksKtMhd2mWyVSkvhDaDLWSc1qYNCz-) | [val_sharp](https://drive.google.com/open?id=1MGeObVQ1-Z29f-myDP7-8c3u0_xECKXq) | test_sharp
Blur | [train_blur](https://drive.google.com/open?id=1Be2cgzuuXibcqAuJekDgvHq4MLYkCgR8) | [val_blur](https://drive.google.com/open?id=1N8z2yD0GDWmh6U4d4EADERtcUgDzGrHx) | [test_blur](https://drive.google.com/file/d/1dr0--ZBKqr4P1M8lek6JKD1Vd6bhhrZT/view?usp=sharing)
Blur + Compression | [train_blur_comp](https://drive.google.com/open?id=1hi6348BB9QQFqVx2PY7pKn32HQM89CJ1) | [val_blur_comp](https://drive.google.com/open?id=13d1uzqLdbsQzeZkWgdF5QVHqDSjfE4zZ) | [test_blur_comp](https://drive.google.com/file/d/1OctyKR3ER_YWrZxKxQsZzLis3BvLSOFO/view?usp=sharing)
Low Resolution | [train_sharp_bicubic](https://drive.google.com/open?id=1a4PrjqT-hShvY9IyJm3sPF0ZaXyrCozR) | [val_sharp_bicubic](https://drive.google.com/open?id=1sChhtzN9Css10gX7Xsmc2JaC-2Pzco6a) | [test_sharp_bicubic](https://drive.google.com/file/d/1y0Jle6xB41TdRK_QMJ_E8W_iBMxwq_Rh/view?usp=sharing)
Blur + Low Resolution | [train_blur_bicubic](https://drive.google.com/open?id=10u8gthv2Q95RMCb1LeCN8N4ozB8TVjMt) | [val_blur_bicubic](https://drive.google.com/open?id=1i3NAb7EmF4fCYadGaHK54-Zgx9lIC2Gp) | [test_blur_bicubic](https://drive.google.com/file/d/14YszfzUAeAfwP0ZA2FRzAiVxxZLg7-tY/view?usp=sharing)

## Updates

We are planning to host an open-end public leaderboard site for the **<font color="red">REDS</font>** related challenges. 
We will provide evaluated PSNR and SSIM for the submitted test results.
Stay tuned for the updates!

## Reference

If you find our dataset useful for your research, please cite our work:

```bibtex
@InProceedings{Nah_2019_CVPR_Workshops,
    author = {Nah, Seungjun and Baik, Sungyong and Hong, Seokil and Moon, Gyeongsik and Son, Sanghyun and Timofte, Radu and Lee, Kyoung Mu},
    title = {NTIRE 2019 Challenge on Video Deblurring and Super-Resolution: Dataset and Study},
    booktitle = {The IEEE Conference on Computer Vision and Pattern Recognition (CVPR) Workshops},
    month = {June},
    year = {2019}
}
```