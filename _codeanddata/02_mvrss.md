---
title: "Multi-View Radar Semantic Segmentation"
excerpt: "<br/><img src='/images/mvrss_teaser.png' width=600px height=auto><br><br><br>"
collection: codeanddata
permalink: /codeanddata/mvrss
---

[Arthur Ouaknine](https://arthurouaknine.github.io/), [Alasdair Newson](https://sites.google.com/site/alasdairnewson/), [Julien Rebut](https://scholar.google.com/citations?user=BJcQNcoAAAAJ&hl=fr), [Florence Tupin](https://perso.telecom-paristech.fr/tupin/), [Patrick Pérez](https://ptrckprz.github.io/)

ICCV 2021.

---

<center><b>Abstract</b></center>

<div style="text-align: justify">Understanding the scene around the ego-vehicle is key to assisted and autonomous driving. Nowadays, this is mostly conducted using cameras and laser scanners, despite their reduced performances in adverse weather conditions. Automotive radars are low-cost active sensors that measure properties of surrounding objects, including their relative speed, and have the key advantage of not being impacted by rain, snow or fog. However, they are seldom used for scene understanding due to the size and complexity of radar raw data and the lack of annotated datasets. Fortunately, recent open-sourced datasets have opened up research on classification, object detection and semantic segmentation with raw radar signals using end-to-end trainable models. In this work, we propose several novel architectures, and their associated losses, which analyse multiple “views” of the range-angle-Doppler radar tensor to segment it semantically. Experiments conducted on the recent CARRADA dataset demonstrate that our best model outperforms alternative models, derived either from the semantic segmentation of natural images or from radar scene understanding, while requiring significantly fewer parameters.</div>

---

<img src='/images/mvrss_teaser.png' class="center">


The **code** and **pretrained models** are available on Github: [https://github.com/valeoai/MVRSS](https://github.com/valeoai/MVRSS)  

The **poster** presented at ICCV is available: [here](https://arthurouaknine.github.io/files/posters/ICCV2021_poster.pdf).  

If you find this code or the dataset useful for your research, please cite our [paper](https://arxiv.org/pdf/2103.16214.pdf):
```
@InProceedings{Ouaknine_2021_ICCV,
	       author = {Ouaknine, Arthur and Newson, Alasdair and P\'erez, Patrick and Tupin, Florence and Rebut, Julien},
               title = {Multi-View Radar Semantic Segmentation},
	       booktitle = {Proceedings of the IEEE/CVF International Conference on Computer Vision (ICCV)},
	       month = {October},
	       year = {2021},
	       pages = {15671-15680}
	       }
```