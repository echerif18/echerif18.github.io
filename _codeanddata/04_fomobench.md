---
title: "FoMo-Bench: a multi-modal, multi-scale and multi-task forest monitoring benchmark for remote sensing foundation models"
excerpt: "<br/><img src='/images/fomobench_teaser.png' width=600px height=auto><br><br><br>"
collection: codeanddata
permalink: /codeanddata/fomobench
---

[Nikolaos Ioannis Bountos](https://ngbountos.github.io/), [Arthur Ouaknine](https://arthurouaknine.github.io/), [David Rolnick](https://davidrolnick.com/)

ArXiv 2023. Under review.  

---

<center><b>Abstract</b></center>

<div style="text-align: justify">
Forests are an essential part of Earth's ecosystems and natural systems, as well as providing services on which humanity depends, yet they are rapidly changing as a result of land use decisions and climate change. Understanding and mitigating negative effects requires parsing data on forests at global scale from a broad array of sensory modalities, and recently many such problems have been approached using machine learning algorithms for remote sensing. To date, forest-monitoring problems have largely been addressed in isolation. Inspired by the rise of foundation models for computer vision and remote sensing, we here present the first unified Forest Monitoring Benchmark (FoMo-Bench). FoMo-Bench consists of 15 diverse datasets encompassing satellite, aerial, and inventory data, covering a variety of geographical regions, and including multispectral, red-green-blue, synthetic aperture radar (SAR) and LiDAR data with various temporal, spatial and spectral resolutions. FoMo-Bench includes multiple types of forest-monitoring tasks, spanning classification, segmentation, and object detection. To further enhance the diversity of tasks and geographies represented in FoMo-Bench, we introduce a novel global dataset, TalloS, combining satellite imagery with ground-based annotations for tree species classification, encompassing 1,000+ categories across multiple hierarchical taxonomic levels (species, genus, family). Finally, we propose FoMo-Net, a baseline foundation model with the capacity to process any combination of commonly used spectral bands in remote sensing, across diverse ground sampling distances and geographical locations worldwide. This work aims to inspire research collaborations between machine learning and forest biology researchers in exploring scalable multi-modal and multi-task models for forest monitoring. All code and data will be made publicly available.</div>

---

<img src='/images/fomobench_teaser.png' class="center">


The **FoMo-Bench** code and data, the **TalloS** dataset and the **FoMo-Net** code and pre-trained models are available on Github: [https://github.com/RolnickLab/FoMo-Bench](https://github.com/RolnickLab/FoMo-Bench)  


If you find our paper, our code or our data useful for your research, please cite our [paper](https://arxiv.org/abs/2312.10114):
```
@misc{bountos2024fomobench,
      title={FoMo-Bench: a multi-modal, multi-scale and multi-task Forest Monitoring Benchmark for remote sensing foundation models}, 
      author={Nikolaos Ioannis Bountos and Arthur Ouaknine and David Rolnick},
      year={2024},
      eprint={2312.10114},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
```