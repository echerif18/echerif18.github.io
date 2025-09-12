---
title: "CARRADA Dataset: Camera and Automotive Radar with Range-Angle-Doppler Annotations"
excerpt: "<br/><img src='/images/carrada.png' width=600px height=auto><br><br><br>"
collection: codeanddata
permalink: /codeanddata/carrada
---

[Arthur Ouaknine](https://arthurouaknine.github.io/), [Alasdair Newson](https://sites.google.com/site/alasdairnewson/), [Julien Rebut](https://scholar.google.com/citations?user=BJcQNcoAAAAJ&hl=fr), [Florence Tupin](https://perso.telecom-paristech.fr/tupin/), [Patrick Pérez](https://ptrckprz.github.io/)

Accepted at ICPR 2020

---

<center><b>Abstract</b></center>

<div style="text-align: justify">High quality perception is essential for autonomous driving (AD) systems. To reach the accuracy and robustness that are required by such systems, several types of sensors must be combined. Currently, mostly cameras and laser scanners (lidar) are deployed to build a representation of the world around the vehicle. While radar sensors have been used for a long time in the automotive industry, they are still under-used for AD despite their appealing characteristics (notably, their ability to measure the relative speed of obstacles and to operate even in adverse weather conditions). To a large extent, this situation is due to the relative lack of automotive datasets with real radar signals that are both raw and annotated. In this work, we introduce CARRADA, a dataset of synchronized camera and radar recordings with range-angle-Doppler annotations. We also present a semi-automatic annotation approach, which was used to annotate the dataset, and a radar semantic segmentation baseline, which we evaluate on several metrics.</div>

---

<img src='/images/carrada.png' class="center">


The **code** is available on Github: [https://github.com/valeoai/carrada_dataset](https://github.com/valeoai/carrada_dataset)

**Access the CARRADA dataset using the following link: [http://download.tsi.telecom-paristech.fr/Carrada](http://download.tsi.telecom-paristech.fr/Carrada).**
- Carrada.tar.gz (23GB): synchronized camera and radar views with generated annotations and materials for the semi-automatic pipeline
- Carrada_RAD.tar.gz (176GB): RAD tensor per sequence only

The **poster** presented at ICPR is available: [here](https://arthurouaknine.github.io/files/posters/ICPR2021_poster.pdf).  

If you find this code or the dataset useful for your research, please cite our [paper](https://arxiv.org/pdf/2005.01456.pdf):
```
@INPROCEEDINGS{9413181,
    author={Ouaknine, Arthur and Newson, Alasdair and Rebut, Julien and Tupin, Florence and Pérez, Patrick},
    booktitle={2020 25th International Conference on Pattern Recognition (ICPR)},
    title={CARRADA Dataset: Camera and Automotive Radar with Range- Angle- Doppler Annotations},
    year={2021},
    volume={},
    number={},
    pages={5068-5075},
    doi={10.1109/ICPR48806.2021.9413181}
}
```