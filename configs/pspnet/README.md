# Pyramid Scene Parsing Network

## Introduction

<!-- [ALGORITHM] -->

<a href="https://github.com/hszhao/PSPNet">Official Repo</a>

<a href="https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/decode_heads/psp_head.py#L63">Code Snippet</a>

<details>
<summary align="right"><a href="https://arxiv.org/abs/1612.01105">PSPNet (CVPR'2017)</a></summary>

```latex
@inproceedings{zhao2017pspnet,
  title={Pyramid Scene Parsing Network},
  author={Zhao, Hengshuang and Shi, Jianping and Qi, Xiaojuan and Wang, Xiaogang and Jia, Jiaya},
  booktitle={CVPR},
  year={2017}
}
```

</details>

## Results and models

### Cityscapes

| Method | Backbone  | Crop Size | Lr schd | Mem (GB) | Inf time (fps) |  mIoU | mIoU(ms+flip) | config                                                                                                                       | download                                                                                                                                                                                                                                                                                                                                                         |
| ------ | --------- | --------- | ------: | -------- | -------------- | ----: | ------------: | ---------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| PSPNet | R-50-D8   | 512x1024  |   40000 | 6.1      | 4.07           | 77.85 |         79.18 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r50-d8_512x1024_40k_cityscapes.py)   | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50-d8_512x1024_40k_cityscapes/pspnet_r50-d8_512x1024_40k_cityscapes_20200605_003338-2966598c.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50-d8_512x1024_40k_cityscapes/pspnet_r50-d8_512x1024_40k_cityscapes_20200605_003338.log.json)         |
| PSPNet | R-101-D8  | 512x1024  |   40000 | 9.6      | 2.68           | 78.34 |         79.74 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r101-d8_512x1024_40k_cityscapes.py)  | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_512x1024_40k_cityscapes/pspnet_r101-d8_512x1024_40k_cityscapes_20200604_232751-467e7cf4.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_512x1024_40k_cityscapes/pspnet_r101-d8_512x1024_40k_cityscapes_20200604_232751.log.json)     |
| PSPNet | R-50-D8   | 769x769   |   40000 | 6.9      | 1.76           | 78.26 |         79.88 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r50-d8_769x769_40k_cityscapes.py)    | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50-d8_769x769_40k_cityscapes/pspnet_r50-d8_769x769_40k_cityscapes_20200606_112725-86638686.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50-d8_769x769_40k_cityscapes/pspnet_r50-d8_769x769_40k_cityscapes_20200606_112725.log.json)             |
| PSPNet | R-101-D8  | 769x769   |   40000 | 10.9     | 1.15           | 79.08 |         80.28 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r101-d8_769x769_40k_cityscapes.py)   | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_769x769_40k_cityscapes/pspnet_r101-d8_769x769_40k_cityscapes_20200606_112753-61c6f5be.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_769x769_40k_cityscapes/pspnet_r101-d8_769x769_40k_cityscapes_20200606_112753.log.json)         |
| PSPNet | R-18-D8   | 512x1024  |   80000 | 1.7      | 15.71          | 74.87 |         76.04 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r18-d8_512x1024_80k_cityscapes.py)   | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r18-d8_512x1024_80k_cityscapes/pspnet_r18-d8_512x1024_80k_cityscapes_20201225_021458-09ffa746.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r18-d8_512x1024_80k_cityscapes/pspnet_r18-d8_512x1024_80k_cityscapes-20201225_021458.log.json)         |
| PSPNet | R-50-D8   | 512x1024  |   80000 | -        | -              | 78.55 |         79.79 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r50-d8_512x1024_80k_cityscapes.py)   | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50-d8_512x1024_80k_cityscapes/pspnet_r50-d8_512x1024_80k_cityscapes_20200606_112131-2376f12b.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50-d8_512x1024_80k_cityscapes/pspnet_r50-d8_512x1024_80k_cityscapes_20200606_112131.log.json)         |
| PSPNet | R-101-D8  | 512x1024  |   80000 | -        | -              | 79.76 |         81.01 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r101-d8_512x1024_80k_cityscapes.py)  | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_512x1024_80k_cityscapes/pspnet_r101-d8_512x1024_80k_cityscapes_20200606_112211-e1e1100f.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_512x1024_80k_cityscapes/pspnet_r101-d8_512x1024_80k_cityscapes_20200606_112211.log.json)     |
| PSPNet (FP16) | R-101-D8 | 512x1024  |   80000 | 5.34     | 8.77           | 79.46 |             - | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r101-d8_fp16_512x1024_80k_cityscapes.py)        | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_fp16_512x1024_80k_cityscapes/pspnet_r101-d8_fp16_512x1024_80k_cityscapes_20200717_230919-a0875e5c.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_fp16_512x1024_80k_cityscapes/pspnet_r101-d8_fp16_512x1024_80k_cityscapes_20200717_230919.log.json)                             |
| PSPNet | R-18-D8   | 769x769   |   80000 | 1.9      | 6.20           | 75.90 |         77.86 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r18-d8_769x769_80k_cityscapes.py)    | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r18-d8_769x769_80k_cityscapes/pspnet_r18-d8_769x769_80k_cityscapes_20201225_021458-3deefc62.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r18-d8_769x769_80k_cityscapes/pspnet_r18-d8_769x769_80k_cityscapes-20201225_021458.log.json)             |
| PSPNet | R-50-D8   | 769x769   |   80000 | -        | -              | 79.59 |         80.69 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r50-d8_769x769_80k_cityscapes.py)    | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50-d8_769x769_80k_cityscapes/pspnet_r50-d8_769x769_80k_cityscapes_20200606_210121-5ccf03dd.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50-d8_769x769_80k_cityscapes/pspnet_r50-d8_769x769_80k_cityscapes_20200606_210121.log.json)             |
| PSPNet | R-101-D8  | 769x769   |   80000 | -        | -              | 79.77 |         81.06 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r101-d8_769x769_80k_cityscapes.py)   | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_769x769_80k_cityscapes/pspnet_r101-d8_769x769_80k_cityscapes_20200606_225055-dba412fa.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_769x769_80k_cityscapes/pspnet_r101-d8_769x769_80k_cityscapes_20200606_225055.log.json)         |
| PSPNet | R-18b-D8  | 512x1024  |   80000 | 1.5      | 16.28          | 74.23 |         75.79 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r18b-d8_512x1024_80k_cityscapes.py)  | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r18b-d8_512x1024_80k_cityscapes/pspnet_r18b-d8_512x1024_80k_cityscapes_20201226_063116-26928a60.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r18b-d8_512x1024_80k_cityscapes/pspnet_r18b-d8_512x1024_80k_cityscapes-20201226_063116.log.json)     |
| PSPNet | R-50b-D8  | 512x1024  |   80000 | 6.0      | 4.30           | 78.22 |         79.46 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r50b-d8_512x1024_80k_cityscapes.py)  | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50b-d8_512x1024_80k_cityscapes/pspnet_r50b-d8_512x1024_80k_cityscapes_20201225_094315-6344287a.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50b-d8_512x1024_80k_cityscapes/pspnet_r50b-d8_512x1024_80k_cityscapes-20201225_094315.log.json)     |
| PSPNet | R-101b-D8 | 512x1024  |   80000 | 9.5      | 2.76           | 79.69 |         80.79 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r101b-d8_512x1024_80k_cityscapes.py) | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101b-d8_512x1024_80k_cityscapes/pspnet_r101b-d8_512x1024_80k_cityscapes_20201226_170012-3a4d38ab.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101b-d8_512x1024_80k_cityscapes/pspnet_r101b-d8_512x1024_80k_cityscapes-20201226_170012.log.json) |
| PSPNet | R-18b-D8  | 769x769   |   80000 | 1.7      | 6.41           | 74.92 |         76.90 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r18b-d8_769x769_80k_cityscapes.py)   | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r18b-d8_769x769_80k_cityscapes/pspnet_r18b-d8_769x769_80k_cityscapes_20201226_080942-bf98d186.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r18b-d8_769x769_80k_cityscapes/pspnet_r18b-d8_769x769_80k_cityscapes-20201226_080942.log.json)         |
| PSPNet | R-50b-D8  | 769x769   |   80000 | 6.8      | 1.88           | 78.50 |         79.96 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r50b-d8_769x769_80k_cityscapes.py)   | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50b-d8_769x769_80k_cityscapes/pspnet_r50b-d8_769x769_80k_cityscapes_20201225_094316-4c643cf6.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50b-d8_769x769_80k_cityscapes/pspnet_r50b-d8_769x769_80k_cityscapes-20201225_094316.log.json)         |
| PSPNet | R-101b-D8 | 769x769   |   80000 | 10.8     | 1.17           | 78.87 |         80.04 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r101b-d8_769x769_80k_cityscapes.py)  | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101b-d8_769x769_80k_cityscapes/pspnet_r101b-d8_769x769_80k_cityscapes_20201226_171823-f0e7c293.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101b-d8_769x769_80k_cityscapes/pspnet_r101b-d8_769x769_80k_cityscapes-20201226_171823.log.json)     |

### ADE20K

| Method | Backbone | Crop Size | Lr schd | Mem (GB) | Inf time (fps) |  mIoU | mIoU(ms+flip) | config                                                                                                                  | download                                                                                                                                                                                                                                                                                                                                     |
| ------ | -------- | --------- | ------: | -------- | -------------- | ----: | ------------: | ----------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| PSPNet | R-50-D8  | 512x512   |   80000 | 8.5      | 23.53          | 41.13 |         41.94 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r50-d8_512x512_80k_ade20k.py)   | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50-d8_512x512_80k_ade20k/pspnet_r50-d8_512x512_80k_ade20k_20200615_014128-15a8b914.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50-d8_512x512_80k_ade20k/pspnet_r50-d8_512x512_80k_ade20k_20200615_014128.log.json)         |
| PSPNet | R-101-D8 | 512x512   |   80000 | 12       | 15.30          | 43.57 |         44.35 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r101-d8_512x512_80k_ade20k.py)  | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_512x512_80k_ade20k/pspnet_r101-d8_512x512_80k_ade20k_20200614_031423-b6e782f0.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_512x512_80k_ade20k/pspnet_r101-d8_512x512_80k_ade20k_20200614_031423.log.json)     |
| PSPNet | R-50-D8  | 512x512   |  160000 | -        | -              | 42.48 |         43.44 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r50-d8_512x512_160k_ade20k.py)  | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50-d8_512x512_160k_ade20k/pspnet_r50-d8_512x512_160k_ade20k_20200615_184358-1890b0bd.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50-d8_512x512_160k_ade20k/pspnet_r50-d8_512x512_160k_ade20k_20200615_184358.log.json)     |
| PSPNet | R-101-D8 | 512x512   |  160000 | -        | -              | 44.39 |         45.35 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r101-d8_512x512_160k_ade20k.py) | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_512x512_160k_ade20k/pspnet_r101-d8_512x512_160k_ade20k_20200615_100650-967c316f.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_512x512_160k_ade20k/pspnet_r101-d8_512x512_160k_ade20k_20200615_100650.log.json) |

### Pascal VOC 2012 + Aug

| Method | Backbone | Crop Size | Lr schd | Mem (GB) | Inf time (fps) |  mIoU | mIoU(ms+flip) | config                                                                                                                   | download                                                                                                                                                                                                                                                                                                                                         |
| ------ | -------- | --------- | ------: | -------- | -------------- | ----: | ------------: | ------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| PSPNet | R-50-D8  | 512x512   |   20000 | 6.1      | 23.59          | 76.78 |         77.61 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r50-d8_512x512_20k_voc12aug.py)  | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50-d8_512x512_20k_voc12aug/pspnet_r50-d8_512x512_20k_voc12aug_20200617_101958-ed5dfbd9.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50-d8_512x512_20k_voc12aug/pspnet_r50-d8_512x512_20k_voc12aug_20200617_101958.log.json)     |
| PSPNet | R-101-D8 | 512x512   |   20000 | 9.6      | 15.02          | 78.47 |         79.25 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r101-d8_512x512_20k_voc12aug.py) | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_512x512_20k_voc12aug/pspnet_r101-d8_512x512_20k_voc12aug_20200617_102003-4aef3c9a.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_512x512_20k_voc12aug/pspnet_r101-d8_512x512_20k_voc12aug_20200617_102003.log.json) |
| PSPNet | R-50-D8  | 512x512   |   40000 | -        | -              | 77.29 |         78.48 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r50-d8_512x512_40k_voc12aug.py)  | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50-d8_512x512_40k_voc12aug/pspnet_r50-d8_512x512_40k_voc12aug_20200613_161222-ae9c1b8c.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50-d8_512x512_40k_voc12aug/pspnet_r50-d8_512x512_40k_voc12aug_20200613_161222.log.json)     |
| PSPNet | R-101-D8 | 512x512   |   40000 | -        | -              | 78.52 |         79.57 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r101-d8_512x512_40k_voc12aug.py) | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_512x512_40k_voc12aug/pspnet_r101-d8_512x512_40k_voc12aug_20200613_161222-bc933b18.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_512x512_40k_voc12aug/pspnet_r101-d8_512x512_40k_voc12aug_20200613_161222.log.json) |

### Pascal Context

| Method | Backbone | Crop Size | Lr schd | Mem (GB) | Inf time (fps) |  mIoU | mIoU(ms+flip) | config                                                                                                                         | download                                                                                                                                                                                                                                                                                                                                                                 |
| ------ | -------- | --------- | ------: | -------- | -------------- | ----: | ------------: | ------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| PSPNet | R-101-D8 | 480x480   |   40000 | 8.8      | 9.68           | 46.60 |         47.78 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r101-d8_480x480_40k_pascal_context.py) | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_480x480_40k_pascal_context/pspnet_r101-d8_480x480_40k_pascal_context_20200911_211210-bf0f5d7c.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_480x480_40k_pascal_context/pspnet_r101-d8_480x480_40k_pascal_context-20200911_211210.log.json) |
| PSPNet | R-101-D8 | 480x480   |   80000 | -        | -              | 46.03 |         47.15 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r101-d8_480x480_80k_pascal_context.py) | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_480x480_80k_pascal_context/pspnet_r101-d8_480x480_80k_pascal_context_20200911_190530-c86d6233.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_480x480_80k_pascal_context/pspnet_r101-d8_480x480_80k_pascal_context-20200911_190530.log.json) |

### Pascal Context 59

| Method | Backbone | Crop Size | Lr schd | Mem (GB) | Inf time (fps) |  mIoU | mIoU(ms+flip) | config                                                                                                                         | download                                                                                                                                                                                                                                                                                                                                                                 |
| ------ | -------- | --------- | ------: | -------- | -------------- | ----: | ------------: | ------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| PSPNet | R-101-D8 | 480x480   |   40000 | -      | -           | 52.02 |         53.54 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r101-d8_480x480_40k_pascal_context_59.py) | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_480x480_40k_pascal_context_59/pspnet_r101-d8_480x480_40k_pascal_context_59_20210416_114524-86d44cd4.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_480x480_40k_pascal_context_59/pspnet_r101-d8_480x480_40k_pascal_context_59-20210416_114524.log.json) |
| PSPNet | R-101-D8 | 480x480   |   80000 | -        | -              | 52.47 |         53.99 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r101-d8_480x480_80k_pascal_context_59.py) | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_480x480_80k_pascal_context_59/pspnet_r101-d8_480x480_80k_pascal_context_59_20210416_114418-fa6caaa2.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_480x480_80k_pascal_context_59/pspnet_r101-d8_480x480_80k_pascal_context_59-20210416_114418.log.json) |

### Dark Zurich and Nighttime Driving

We support evaluation results on these two datasets using models above trained on Cityscapes training set.

  |Method|Backbone |Training Dataset |Test Dataset          |mIoU |config| evaluation checkpoint|
  |------ |------  |------ |-----            |-----|-----|-----|
  |PSPNet|R-50-D8  |Cityscapes Training set |Dark Zurich      |10.91|[config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r50-d8_512x1024_40k_dark.py)|[model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50-d8_512x1024_40k_cityscapes/pspnet_r50-d8_512x1024_40k_cityscapes_20200605_003338-2966598c.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50-d8_512x1024_40k_cityscapes/pspnet_r50-d8_512x1024_40k_cityscapes_20200605_003338.log.json) |
  |PSPNet|R-50-D8  |Cityscapes Training set |Nighttime Driving|23.02|[config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r50-d8_512x1024_40k_night_driving.py)| [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50-d8_512x1024_40k_cityscapes/pspnet_r50-d8_512x1024_40k_cityscapes_20200605_003338-2966598c.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50-d8_512x1024_40k_cityscapes/pspnet_r50-d8_512x1024_40k_cityscapes_20200605_003338.log.json) |
  |PSPNet|R-50-D8  |Cityscapes Training set |Cityscapes Validation set|77.85 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r50-d8_512x1024_40k_cityscapes.py)   | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50-d8_512x1024_40k_cityscapes/pspnet_r50-d8_512x1024_40k_cityscapes_20200605_003338-2966598c.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50-d8_512x1024_40k_cityscapes/pspnet_r50-d8_512x1024_40k_cityscapes_20200605_003338.log.json) |
  |PSPNet|R-101-D8 |Cityscapes Training set |Dark Zurich      |10.16|[config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r101-d8_512x1024_40k_dark.py)| [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_512x1024_40k_cityscapes/pspnet_r101-d8_512x1024_40k_cityscapes_20200604_232751-467e7cf4.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_512x1024_40k_cityscapes/pspnet_r101-d8_512x1024_40k_cityscapes_20200604_232751.log.json) |
  |PSPNet|R-101-D8 |Cityscapes Training set |Nighttime Driving|20.25|[config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r101-d8_512x1024_40k_night_driving.py)| [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_512x1024_40k_cityscapes/pspnet_r101-d8_512x1024_40k_cityscapes_20200604_232751-467e7cf4.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_512x1024_40k_cityscapes/pspnet_r101-d8_512x1024_40k_cityscapes_20200604_232751.log.json) |
  |PSPNet|R-101-D8 |Cityscapes Training set |Cityscapes Validation set|78.34|[config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r101-d8_512x1024_40k_cityscapes.py)  | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_512x1024_40k_cityscapes/pspnet_r101-d8_512x1024_40k_cityscapes_20200604_232751-467e7cf4.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_512x1024_40k_cityscapes/pspnet_r101-d8_512x1024_40k_cityscapes_20200604_232751.log.json)     |
  |PSPNet|R-101b-D8|Cityscapes Training set |Dark Zurich      |15.54|[config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r101b-d8_512x1024_80k_dark.py)| [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101b-d8_512x1024_80k_cityscapes/pspnet_r101b-d8_512x1024_80k_cityscapes_20201226_170012-3a4d38ab.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101b-d8_512x1024_80k_cityscapes/pspnet_r101b-d8_512x1024_80k_cityscapes-20201226_170012.log.json) |
  |PSPNet|R-101b-D8|Cityscapes Training set |Nighttime Driving|22.25|[config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r101b-d8_512x1024_80k_night_driving.py)| [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101b-d8_512x1024_80k_cityscapes/pspnet_r101b-d8_512x1024_80k_cityscapes_20201226_170012-3a4d38ab.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101b-d8_512x1024_80k_cityscapes/pspnet_r101b-d8_512x1024_80k_cityscapes-20201226_170012.log.json) |
  |PSPNet|R-101b-D8|Cityscapes Training set |Cityscapes Validation set|79.69|[config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet/pspnet_r101b-d8_512x1024_80k_cityscapes.py) | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101b-d8_512x1024_80k_cityscapes/pspnet_r101b-d8_512x1024_80k_cityscapes_20201226_170012-3a4d38ab.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101b-d8_512x1024_80k_cityscapes/pspnet_r101b-d8_512x1024_80k_cityscapes-20201226_170012.log.json) |

### COCO-Stuff 10k

| Method    | Backbone | Crop Size | Lr schd | Mem (GB) | Inf time (fps) |  mIoU | mIoU(ms+flip) | config                                                                                                                        | download                                                                                                                                                                                                                                                                                                                                                       |
| --------- | -------- | --------- | ------: | -------- | -------------- | ----: | ------------: | ----------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| PSPNet | R-50-D8  | 512x512   |   20000 | 9.6      | 20.5          | 35.69 |         36.62 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet_r50-d8_512x512_4x4_20k_coco-stuff10k.py)   | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50-d8_512x512_4x4_20k_coco-stuff10k/pspnet_r50-d8_512x512_4x4_20k_coco-stuff10k_20210820_203258-b88df27f.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50-d8_512x512_4x4_20k_coco-stuff10k/pspnet_r50-d8_512x512_4x4_20k_coco-stuff10k_20210820_203258.log.json)         |
| PSPNet | R-101-D8 | 512x512   |   20000 | 13.2     | 11.1          | 37.26 |         38.52 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet_r101-d8_512x512_4x4_20k_coco-stuff10k.py)  | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_512x512_4x4_20k_coco-stuff10k/pspnet_r101-d8_512x512_4x4_20k_coco-stuff10k_20210820_232135-76aae482.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_512x512_4x4_20k_coco-stuff10k/pspnet_r101-d8_512x512_4x4_20k_coco-stuff10k_20210820_232135.log.json)     |
| PSPNet | R-50-D8  | 512x512   |  40000 | -        | -              | 36.33 |         37.24 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet_r50-d8_512x512_4x4_40k_coco-stuff10k.py)  | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50-d8_512x512_4x4_40k_coco-stuff10k/pspnet_r50-d8_512x512_4x4_40k_coco-stuff10k_20210821_030857-92e2902b.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50-d8_512x512_4x4_40k_coco-stuff10k/pspnet_r50-d8_512x512_4x4_40k_coco-stuff10k_20210821_030857.log.json)     |
| PSPNet | R-101-D8 | 512x512   |  40000 | -        | -              | 37.76 |         38.86 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet_r101-d8_512x512_4x4_40k_coco-stuff10k.py) | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_512x512_4x4_40k_coco-stuff10k/pspnet_r101-d8_512x512_4x4_40k_coco-stuff10k_20210821_014022-831aec95.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_512x512_4x4_40k_coco-stuff10k/pspnet_r101-d8_512x512_4x4_40k_coco-stuff10k_20210821_014022.log.json) |

### COCO-Stuff 164k

| Method    | Backbone | Crop Size | Lr schd | Mem (GB) | Inf time (fps) |  mIoU | mIoU(ms+flip) | config                                                                                                                        | download                                                                                                                                                                                                                                                                                                                                                       |
| --------- | -------- | --------- | ------: | -------- | -------------- | ----: | ------------: | ----------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| PSPNet | R-50-D8  | 512x512   |   80000 | 9.6      | 20.5          | 38.80 |         39.19 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet_r50-d8_512x512_4x4_80k_coco-stuff164k.py)   | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50-d8_512x512_4x4_80k_coco-stuff164k/pspnet_r50-d8_512x512_4x4_80k_coco-stuff164k_20210707_152034-0e41b2db.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50-d8_512x512_4x4_80k_coco-stuff164k/pspnet_r50-d8_512x512_4x4_80k_coco-stuff164k_20210707_152034.log.json)         |
| PSPNet | R-101-D8 | 512x512   |   80000 | 13.2     | 11.1          | 40.34 |         40.79 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet_r101-d8_512x512_4x4_80k_coco-stuff164k.py)  | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_512x512_4x4_80k_coco-stuff164k/pspnet_r101-d8_512x512_4x4_80k_coco-stuff164k_20210707_152034-7eb41789.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_512x512_4x4_80k_coco-stuff164k/pspnet_r101-d8_512x512_4x4_80k_coco-stuff164k_20210707_152034.log.json)     |
| PSPNet | R-50-D8  | 512x512   |  160000 | -        | -              | 39.64 |         39.97 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet_r50-d8_512x512_4x4_160k_coco-stuff164k.py)  | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50-d8_512x512_4x4_160k_coco-stuff164k/pspnet_r50-d8_512x512_4x4_160k_coco-stuff164k_20210707_152004-51276a57.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50-d8_512x512_4x4_160k_coco-stuff164k/pspnet_r50-d8_512x512_4x4_160k_coco-stuff164k_20210707_152004.log.json)     |
| PSPNet | R-101-D8 | 512x512   |  160000 | -        | -              | 41.28 |         41.66 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet_r101-d8_512x512_4x4_160k_coco-stuff164k.py) | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_512x512_4x4_160k_coco-stuff164k/pspnet_r101-d8_512x512_4x4_160k_coco-stuff164k_20210707_152004-4af9621b.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_512x512_4x4_160k_coco-stuff164k/pspnet_r101-d8_512x512_4x4_160k_coco-stuff164k_20210707_152004.log.json) |
| PSPNet | R-50-D8  | 512x512   |  320000 | -        | -              | 40.53 |         40.75 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet_r50-d8_512x512_4x4_320k_coco-stuff164k.py)  | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50-d8_512x512_4x4_320k_coco-stuff164k/pspnet_r50-d8_512x512_4x4_320k_coco-stuff164k_20210707_152004-be9610cc.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r50-d8_512x512_4x4_320k_coco-stuff164k/pspnet_r50-d8_512x512_4x4_320k_coco-stuff164k_20210707_152004.log.json)     |
| PSPNet | R-101-D8 | 512x512   |  320000 | -        | -              | 41.95 |         42.42 | [config](https://github.com/open-mmlab/mmsegmentation/blob/master/configs/pspnet_r101-d8_512x512_4x4_320k_coco-stuff164k.py) | [model](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_512x512_4x4_320k_coco-stuff164k/pspnet_r101-d8_512x512_4x4_320k_coco-stuff164k_20210707_152004-72220c60.pth) &#124; [log](https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_512x512_4x4_320k_coco-stuff164k/pspnet_r101-d8_512x512_4x4_320k_coco-stuff164k_20210707_152004.log.json) |

Note:

- `FP16` means Mixed Precision (FP16) is adopted in training.