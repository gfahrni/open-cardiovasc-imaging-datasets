# Open Cardiovascular Imaging Datasets — Catalog

A curated catalog of publicly available datasets for cardiovascular imaging, compiled as part of a scoping review published in *European Radiology — Cardiovascular and Thoracic* (2026).

This repository provides a living, searchable reference for researchers working on AI/deep learning in cardiovascular imaging. The full metadata (all fields, acquisition parameters, features) is available in [`catalog.csv`](./data/catalog.csv).

> **Cite this catalog:**  
> [Author et al. (2026). *Open-Access Datasets for Cardiovascular Imaging: A Scoping Review.* European Radiology — Cardiovascular and Thoracic.] — DOI: `[to fill]`  
> Zenodo snapshot: `[DOI to fill after deposit]`

---

## Summary

| Domain | n datasets | Modalities |
|---|---|---|
| Coronary Arteries | 5 | CT |
| Aorta | 4 | CT |
| Heart | 16 | CT, MRI, US |
| Pulmonary Arteries | 6 | CT |
| Peripheral Arteries | 3 | CT, US |
| Multi-Organ | 4 | CT, MRI |
| **Total** | **39** | |

---

## Coronary Arteries

| Name | Task | Modality | n | Date | Size | License | Platform | Strengths |
|---|---|---|---|---|---|---|---|---|
| [ImageCAS](https://www.kaggle.com/datasets/xiaoweixumedicalai/imagecas) | Coronary artery segmentation | CT | 1,000 CCTA | 2023 | 89.1 GB | Apache 2.0 | Kaggle | Largest 3D coronary CCTA dataset; public benchmark with baseline model |
| [ImageALCAPA](https://www.kaggle.com/datasets/xiaoweixumedicalai/imagealcapa) | ALCAPA anatomy segmentation | CT | 30 CCTA | 2022 | 2.6 GB | Apache 2.0 | Kaggle | First public dataset for ALCAPA; supports 3D printing for surgical planning |
| [COCA](https://stanfordaimi.azurewebsites.net/datasets/e8ca74dc-8dd4-4340-815a-60b41f6cb2aa) | CAC scoring & segmentation | CT | 425 + 199 | 2021 | 28 GB | Stanford DUA | Stanford AIMI | Dual-cohort (gated + non-gated); DICOM + segmentations + CAC scores |
| [3D CAS Images](https://www.kaggle.com/datasets/ahanafabidsazid/3d-cat-images) | Coronary artery segmentation | CT | 200 | 2025 | 135 GB | Apache 2.0 | Kaggle | Voxel-level artery segmentation; NIfTI format |
| [MultiD4CAD](https://zenodo.org/records/15148653) | CAD diagnosis & EAT/PAT segmentation | CT | 118 CCTA | 2025 | 4.0 TB | DUA | Zenodo | First multimodal CCTA + clinical risk factors dataset; expert-validated annotations |

---

## Aorta

| Name | Task | Modality | n | Date | Size | License | Platform | Strengths |
|---|---|---|---|---|---|---|---|---|
| [ImageTBAD](https://www.kaggle.com/datasets/xiaoweixumedicalai/imagetbad) | Type B aortic dissection segmentation | CT | 100 CTA | 2021 | 13.4 GB | Apache 2.0 | Kaggle | First 3D TBAD dataset with FLT annotation; dual-radiologist annotation |
| [AVT](https://doi.org/10.6084/m9.figshare.14806362) | Aortic vessel tree segmentation | CT | 56 CTA | 2022 | 5.8 GB | CC BY 4.0 | Figshare | Multicenter (3 sources); full aortic tree arch to iliac; includes AAA and AD |
| [AortaSeg-60](https://doi.org/10.5281/zenodo.18147026) | Aortic segmentation | CT | 60 CTA | 2026 | 15.9 GB | CC0 1.0 | Zenodo | Most permissive license (CC0); 6 pathological subsets including normal controls |
| [ImageTAAD](https://www.kaggle.com/datasets/xiaoweixumedicalai/imagetaad) | Type A aortic dissection segmentation | CT | 120 CTA | 2025 | 26.9 GB | Apache 2.0 | Kaggle | First comprehensive TAAD dataset; 35 annotated categories; clinical evaluation metrics |

---

## Heart

| Name | Task | Modality | n | Date | Size | License | Platform | Strengths |
|---|---|---|---|---|---|---|---|---|
| [HVSMR-2.0](https://figshare.com/collections/HVSMR-2_0_A_3D_cardiovascular_MR_dataset_for_whole-heart_segmentation_in_congenital_heart_disease/7074755/2) | Whole-heart & great vessel segmentation | MRI | 60 | 2024 | 1.6 GB | CC BY 4.0 | Figshare | Focus on CHD; high anatomical variability; 8 structure labels |
| [ACDC](https://www.kaggle.com/datasets/anhoangvo/acdc-dataset) | Cardiac structure segmentation (LV, RV, MYO) | MRI | 150 | 2018 | 0.3 GB | MIT | Kaggle | Established benchmark; scribble annotations for weakly supervised learning |
| [CAMUS](https://humanheart-project.creatis.insa-lyon.fr/database/#collection/6373703d73e9f0047faa1bc8) | Multi-structure segmentation (LV, Myo, LA) | US | 500 | 2019 | 3.6 GB | CC BY-NC-SA 4.0 | Human Heart Project | High clinical realism; includes poor-quality cases; EF labels |
| [EchoNet-Dynamic](https://stanfordaimi.azurewebsites.net/datasets/echonet-dynamic) | EF estimation & LV segmentation | US | 10,030 videos | 2020 | 5 GB | Stanford DUA | Stanford AIMI | Largest labeled echo video dataset; expert tracings; EF/ESV/EDV labels |
| [CardiacUDA](https://www.kaggle.com/datasets/xiaoweixumedicalai/cardiacudc-dataset) | Cardiac structure segmentation & UDA | US | 992 videos | 2023 | 4.5 GB | Apache 2.0 | Kaggle | First UDA benchmark for echo segmentation; multi-center (2 hospitals) |
| [CHD68](https://www.kaggle.com/datasets/xiaoweixumedicalai/chd68-segmentation-dataset-miccai19) | Whole-heart segmentation in CHD | CT | 68 | 2019 | 5.4 GB | Apache 2.0 | Kaggle | First public CHD whole-heart dataset; 14 CHD types; paediatric population |
| [ImageCHD](https://www.kaggle.com/datasets/xiaoweixumedicalai/imagechd) | CHD classification & segmentation | CT | 110 | 2021 | 9.8 GB | Apache 2.0 | Kaggle | 16 CHD types; combined segmentation + classification labels |
| [EchoCP](https://www.kaggle.com/datasets/xiaoweixumedicalai/echocp/data) | PFO diagnosis & cardiac chamber segmentation | US | 60 videos | 2021 | 1.2 GB | Apache 2.0 | Kaggle | First contrast TTE dataset for PFO; rest + Valsalva states per patient |
| [EchoNet-LVH](https://echonet.github.io/lvh/index.html) | LVH quantification & etiology classification | US | 12,000 videos | 2022 | ~5 GB | Stanford DUA | Stanford AIMI | Large-scale PLAX dataset; expert-verified measurements; HCM/amyloidosis/HTN/AS labels |
| [EchoNet-Pediatric](https://echonet.github.io/pediatric) | LV function analysis | US | 7,643 videos | 2024 | 2.51 GB | Stanford DUA | Stanford AIMI | First large-scale paediatric echo dataset; 0–18 yrs; oncology + heart failure cohorts |
| [EchoNet-TEE](https://aimi.stanford.edu/datasets/echonet-tee-view-classifier) | TEE view classification | US | 465 videos | 2024 | ~40 GB | Stanford DUA | Stanford AIMI | First public intraoperative TEE dataset; 8 standardized view classes |
| [Sunnybrook Cardiac MRI](https://www.cardiacatlas.org/sunnybrook-cardiac-data/) | LV segmentation & function quantification | MRI | 45 | 2009 | 2.7 GB | CC BY 4.0 | Cardiac Atlas | First standardized LV benchmark; 4 pathology groups including normal |
| [3C](https://doi.org/10.5281/zenodo.10801492) | Cardiac complication detection in COVID-19 | CT | 134 | 2024 | 43.9 GB | CC BY 4.0 | Zenodo | First dataset linking CT findings to COVID-19 cardiac complications; wide age range |
| [OCMR](https://ocmr.s3.amazonaws.com/data/ocmr_cine.tar.gz) | Cardiac cine MRI reconstruction | MRI | 265 series | 2020 | 123 GB | CC BY 4.0 | AWS S3 | Only public multi-coil k-space dataset for cardiac MRI; 1.5T & 3T scanners |
| [Cardiac Atlas Project](https://www.cardiacatlas.org) | Shape modeling & LV segmentation | MRI | ~3,000 | 2011 | ~600 GB | CC BY-NC 2.5 | Cardiac Atlas | Largest cardiac MRI resource; MESA + DETERMINE cohorts; clinical metadata |
| [HOCMvalvesSeg](https://www.kaggle.com/datasets/xiaoweixumedicalai/hocmvalvesseg) | Aortic/mitral valve & heart structure segmentation | CT | 27 | 2023 | 6.5 GB | Apache 2.0 | Kaggle | First valve segmentation dataset for HOCM; supports surgical planning |

---

## Pulmonary Arteries

| Name | Task | Modality | n | Date | Size | License | Platform | Strengths |
|---|---|---|---|---|---|---|---|---|
| [RSPECT](https://www.kaggle.com/c/rsna-str-pulmonary-embolism-detection/data) | PE detection, classification & quantification | CT | 12,195 CTPA | 2021 | 980.2 GB | Non-commercial research only | Kaggle | Largest PE dataset; 86 subspecialist radiologists; 5 countries; rich study-level labels |
| [Radfusion](https://stanfordaimi.azurewebsites.net/datasets/3a7548a4-8f65-4ab7-85fa-3d68c9efc1bd) | PE detection & fairness evaluation | CT | 1,837 CTPA | 2021 | ~300 GB | Stanford DUA | Stanford AIMI | First CT + longitudinal EHR dataset for PE; fairness evaluation included |
| [FUMPE](https://www.kaggle.com/datasets/andrewmvd/pulmonary-embolism-in-ct-images) | PE detection & segmentation | CT | 35 CTPA | 2018 | 4.6 GB | N/A | Kaggle | Pixel-level PE ground truth; dual expert annotation; early reference dataset |
| [INSPECT](https://stanfordaimi.azurewebsites.net/datasets?term=INSPECT) | PE diagnosis & prognosis (multimodal) | CT | 23,248 CTPA | 2023 | ~2.5 TB | Stanford DUA | Stanford AIMI | Largest dataset in catalog; CTPA + radiology reports + full EHR (OMOP) |
| [ChestPathCT5-S100](https://zenodo.org/records/18256797) | Thoracic pathology classification | CT | 87 | 2026 | 9.6 GB | CC0 1.0 | Zenodo | Multi-pathology (PE, pneumothorax, pleural fluid, pulmonary mass); CC0 license |
| [ImageVessel](https://www.kaggle.com/datasets/xiaoweixumedicalai/mytest) | Pulmonary artery & vein segmentation | CT | 95 | 2024 | 19.7 GB | Apache 2.0 | Kaggle | First public pulmonary artery/vein segmentation dataset; surgical planning focus |

---

## Peripheral Arteries

| Name | Task | Modality | n | Date | Size | License | Platform | Strengths |
|---|---|---|---|---|---|---|---|---|
| [CUBS](https://doi.org/10.17632/m7ndn58sv6.1) | Carotid IMT measurement & segmentation | US | 500 images | 2022 | 0.1 GB | CC BY 4.0 | Mendeley Data | Multicenter benchmark; 7 automated algorithms vs 3 expert annotations |
| [Common Carotid Artery US](https://doi.org/10.17632/d4xt63mgjm.1) | Carotid artery segmentation | US | 1,100 images | 2022 | 0.2 GB | CC BY 4.0 | Mendeley Data | Expert segmentation masks; simple accessible format |
| [KiPA22](https://kipa22.grand-challenge.org) | Kidney, renal artery & vein segmentation | CT | 130 CTA | 2022 | ~6.5 GB | CC BY-NC-ND | Grand Challenge | Only public dataset with annotated renal artery + vein; includes tumors |

---

## Multi-Organ

| Name | Task | Modality | n | Date | Size | License | Platform | Strengths |
|---|---|---|---|---|---|---|---|---|
| [TotalSegmentator CT](https://doi.org/10.5281/zenodo.6802614) | Whole-body segmentation (117 structures) | CT | 1,228 | 2023 | 23.6 GB | Apache 2.0 | Zenodo | Largest multi-organ CT dataset; includes all major cardiovascular structures |
| [Medical Segmentation Decathlon](http://medicaldecathlon.com/) | Multi-organ segmentation (10 tasks) | CT, MRI | 2,633 | 2022 | 97.5 GB | CC BY-SA 4.0 | AWS Open Data | Cross-task generalizability benchmark; includes cardiac (left atrium) task |
| [TotalSegmentator MRI](https://doi.org/10.5281/zenodo.14710732) | Whole-body segmentation (50 structures) | MRI | 616 | 2025 | 5.1 GB | Apache 2.0 | Zenodo | Largest multi-organ MRI dataset; real-world clinical data |
| [AortaSeg24](https://aortaseg24.grand-challenge.org/) | Aortic branches & zones segmentation | CT | 100 CTA | 2025 | ~50 GB | DUA | Grand Challenge | 23 aortic branches + SVS/STS zones; expert vascular surgeon annotations |

---

## License distribution

| License | n |
|---|---|
| Apache 2.0 | 12 |
| Stanford DUA | 5 |
| CC BY 4.0 | 5 |
| CC BY-NC variants | 3 |
| CC0 | 2 |
| DUA (other) | 2 |
| Non-commercial only | 1 |
| No license stated | 1 |

---

## How to cite

If you use this catalog, please cite both the article and the Zenodo snapshot:

```
[Author et al. (2026). Open-Access Datasets for Cardiovascular Imaging: A Scoping Review.
European Radiology — Cardiovascular and Thoracic. DOI: to fill]

[Zenodo catalog snapshot. DOI: to fill]
```

---

## Contributing

Found a missing dataset? Open an issue or submit a pull request.  
Please include: Name, Task, Modality, n, Date, Size, License, Platform, URL.

---

*Last updated: March 2026*
