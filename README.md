# Utils for using MMSegmentation framework for asbestos veins segmentation problem in open-pit conditions

## Data

The dataset of images of stone fragments with asbestos veins in open-pit conditions is available at https://urfume-my.sharepoint.com/:f:/g/personal/v_e_misilov_urfu_me/EuDsCAkxMuBLstYwQEEBltMB7BdSc9VdhGbih0wXSSRnQw?e=9ZPKwT

## Baseline results 

Trained data is available at https://urfume-my.sharepoint.com/:f:/g/personal/v_e_misilov_urfu_me/EoH88vyEXnNOujxNHTvMvRYBX7Hy3PUSZA5zh8mRvQ1o4Q?e=77nmFh

**U-Net**: *unet-s5-d16_fcn_4xb4-160k_cityscapes-512x1024*

|   Class    |  IoU  |  Acc  |  Dice | Fscore | Precision | Recall |
|------------|-------|-------|-------|--------|-----------|--------|
| background |  0.0  |  nan  |  0.0  |  nan   |    0.0    |  nan   |
|   stone    | 77.76 | 78.37 | 87.49 | 87.49  |   99.01   | 78.37  |
|  asbestos  |  5.08 | 48.38 |  9.66 |  9.66  |    5.37   | 48.38  |

**Segformer**: *segformer_mit-b4_8xb1-160k_cityscapes-1024x1024*

|   Class    |  IoU  |  Acc  |  Dice | Fscore | Precision | Recall |
|------------|-------|-------|-------|--------|-----------|--------|
| background |  0.0  |  nan  |  0.0  |  nan   |    0.0    |  nan   |
|   stone    | 86.12 | 86.53 | 92.54 | 92.54  |   99.45   | 86.53  |
|  asbestos  | 20.68 | 71.97 | 34.27 | 34.27  |   22.49   | 71.97  |
