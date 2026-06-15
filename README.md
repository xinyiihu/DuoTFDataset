# Datasets for DuoTransFormer

## Introduction

This is the official repository for the DuoTransFormer datasets: [DuoTransFormer for nonlinear seismic response prediction: Cover large, focus local, and enforce law](https://www.sciencedirect.com/science/article/abs/pii/S1474034626000674).

In this study, we develop a novel dual-view Transformer-based model framework for nonlinear seismic response prediction. It predicts multivariate structural nonlinear response quantities in a time-aligned manner, including base shear, acceleration, velocity, and displacement.

## Data

The four datasets used in the paper, namely MDOFe, MDOFn, TBI2A, and SHT, are provided in the [`datasets/`](datasets/) folder. MDOFe, MDOFn, and TBI2A use the same 97 selected ground motion records, while SHT uses a different set of 35 selected ground motion records. Each CSV file contains the corresponding ground motion record and the response variables under that seismic excitation. Please refer to Section 4.2.2 of the paper for the detailed composition of the response variables.

| Dataset | Folder | Number of CSV files | Main contents |
| --- | --- | ---: | --- |
| MDOFe | `datasets/1_MDOFe/` | 97 | `time`, `GM_main`, `baseforce`, and selected `acc_*`, `vel_*`, and `dis_*` response columns |
| MDOFn | `datasets/2_MDOFn/` | 97 | `time`, `GM_main`, `baseforce`, and selected `acc_*`, `vel_*`, and `dis_*` response columns |
| TBI2A | `datasets/3_TBI2A/` | 97 | `time`, three-component ground motions, `baseforce`, and selected `acc_*`, `vel_*`, and `dis_*` response columns |
| SHT | `datasets/4_SHT/` | 35 | `time`, three-component ground motions, `baseforce`, roof acceleration, and `dis_*` response columns |

![Information of selected ground motion records for the MDOF models and TBI2A case](pic/Table%20B.8.png)

*Table B.8. Information of selected ground motion records for the MDOF models and TBI2A case.*

![Information of selected ground motion records for the Shanghai Tower case](pic/Table%20B.9.png)

*Table B.9. Information of selected ground motion records for the Shanghai Tower case.*

## Citation

If you find this repository useful in your research, please consider citing the following paper:

```bibtex
@article{hu2026duotransformer,
  title={DuoTransFormer for nonlinear seismic response prediction: Cover large, focus local, and enforce law},
  author={Hu, Xinyi and Xiao, Congzhen and Zhang, Zhiqiang and Gao, Jie},
  journal={Advanced Engineering Informatics},
  volume={71},
  pages={104375},
  year={2026},
  publisher={Elsevier}
}
```

## Contact

If you have any questions, feel free to contact Xinyi Hu through Email (xiny.hu@outlook.com).
