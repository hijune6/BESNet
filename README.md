# Boundary Enhancing Semantic Context Network for Parsing High-resolution Remote Sensing Images
- Updating......

The code is based on FCN_8s

# Datasets
- ISPRS [Vaihingen](https://www2.isprs.org/commissions/comm2/wg4/benchmark/2d-sem-label-vaihingen/) dataset
- ISPRS [Potsdam](https://www2.isprs.org/commissions/comm2/wg4/benchmark/2d-sem-label-potsdam/) dataset
- The original dataset can be requested for the download from [here](https://www2.isprs.org/commissions/comm2/wg4/benchmark/data-request-form/).
- You should cut the training images as well as corresponding labels into patches with an overlap of 171 pixels.

# Requiements
- Python == 3.7.10
- PyTorch == 1.8.1
- CUDA ==10.1

# Train
For Vaihingen, run:
```
sh train_vaihingen_fcn.sh
```
For Potsdam, run:
```
sh train_potsdam_fcn.sh
```
The results will be saved in the `./snapshots/` folder.

# Test
For test, run:
```
sh Eval.sh
```
For different datasets, please manully change `dataset` in `Eval.sh`.

# Citation
Please kindly cite the following paper in your publications if it helps your research:
```
@article{Chen2022BESNetBE,
  title={BES-Net: Boundary Enhancing Semantic Context Network for High-Resolution Image Semantic Segmentation},
  author={Fenglei Chen and Haijun Liu and Zhihong Zeng and Xichuan Zhou and Xiaoheng Tan},
  journal={Remote Sensing},
  year={2022},
  volume={14},
  pages={1638}
}
```
