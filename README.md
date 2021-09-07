# cluster_buster

fMRI studies sometimes yield very large clusters of voxels that are hard to precisely label.

![activation](https://user-images.githubusercontent.com/5094574/132413664-5a70218e-0f54-4f1f-a293-89f156c46f8f.png)

This jupyter notebook will take stat maps inside the input folder and create a table with voxel counts for different cortical, subcortical, and cerebellar ROIs. For example, the script will break a large cluster into smaller subunits based on the Harvard-Oxford labels. Atlas image:

![atlas](https://user-images.githubusercontent.com/5094574/132413687-a29a20b8-965c-4b49-9906-e0e42271557e.png)

The final product is a table formed from voxel counts of the parcelled activation map.

![activation_parcels](https://user-images.githubusercontent.com/5094574/132413680-81e5f0be-3266-4597-9441-92f47bc59548.png)

| Region                                                               | Cluster 1 Voxel Count |
|                                                                 ---: |                  ---: |
| Frontal Pole                                                         |                  4489 |
| Insular Cortex                                                       |                   615 |
| Superior Frontal Gyrus                                               |                  2952 |
| Middle Frontal Gyrus                                                 |                  3821 |
| Inferior Frontal Gyrus, pars triangularis                            |                   509 |
| Inferior Frontal Gyrus, pars opercularis                             |                  1302 |
| Precentral Gyrus                                                     |                  1406 |
| Juxtapositional Lobule Cortex (formerly Supplementary Motor Cortex)  |                   308 |
| Paracingulate Gyrus                                                  |                  1578 |
| Cingulate Gyrus, anterior division                                   |                   804 |
| Frontal Orbital Cortex                                               |                   995 |
| Frontal Operculum Cortex                                             |                   516 |
| Left Lateral Ventrical                                               |                    65 |
| Left Thalamus                                                        |                   145 |
| Left Caudate                                                         |                   343 |
| Left Putamen                                                         |                   217 |
| Brain-Stem                                                           |                    60 |
| Right Lateral Ventricle                                              |                    56 |
| Right Thalamus                                                       |                   226 |
| Right Caudate                                                        |                   344 |
| Right Putamen                                                        |                   166 |

Works best with Pandas > version 1.3. Requires an install of FSL.

Provided with example data from Reineberg et al. (in revision). The neural basis of individual differences in general executive function: Context-specific activation modulated by frontal cortex connectivity.