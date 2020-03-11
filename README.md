## Pytorch1.4-WCT-Universal Style Transfer
This is the Pytorch1.4 version of [Universal Style Transfer via Feature Transforms](https://arxiv.org/pdf/1705.08086.pdf).

We translated the original [WCT code](https://github.com/sunshineatnoon/PytorchWCT) from Pytorch 0.4.1 to Pytorch 1.4. Details of the code refers to https://github.com/sunshineatnoon/PytorchWCT.

## Prerequisites
- [Pytorch 1.4](http://pytorch.org/)
- [torchvision 0.5.0](https://github.com/pytorch/vision)
- Pretrained encoder and decoder [models](https://drive.google.com/file/d/1M5KBPfqrIUZqrBZf78CIxLrMUT4lD4t9/view?usp=sharing) for image reconstruction only (download and uncompress them under models/). **The .t7 files must convert to .pth with [Convert code](https://github.com/clcarwin/convert_torch_to_pytorch).**
- CUDA + CuDNN

## Prepare images
Simply put content and image pairs in `images/content` and `images/style` respectively. Note that correspoding conternt and image pairs should have same names.


## Style Transfer

```
python WCT.py --cuda
```
### Reference
Li Y, Fang C, Yang J, et al. Universal Style Transfer via Feature Transforms[J]. arXiv preprint arXiv:1705.08086, 2017.
