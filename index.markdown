
---
layout: default
title: "Visual-textual Dermatoglyphic Animal Biometrics: A First Case Study on Panthera tigris"
---

### **Overview**

Biologists have long combined photographs and sketches with textual field notes to re-identify (Re-ID) individual animals based on phenotypic traits. Contemporary AI-supported camera trapping builds on this visual tradition, with computer vision tools now supporting animal re-identification across numerous species with distinctive morphological features, such as unique stripe-like coats (e.g., zebras, tigers). Here, we present the first study to extend image-only Re-ID methodologies by incorporating precise dermatoglyphic textual descriptors -- an approach widely used in forensic science but hitherto unexploited in ecology. We demonstrate that these specialist semantics can abstract and encode both the topology and structure of animal stripe coats using fully human-interpretable language tags. Drawing on 84,264 manually labelled minutiae features across 3,355 images of 185 individual tigers (Panthera tigris), we provide a comprehensive quantitative case study evaluating this new visual–textual methodology in detail, revealing novel capabilities for cross-modal dermatoglyphic animal identity retrieval. To optimise performance we synthesise 2,000 ‘virtual individuals’ multimodally, each comprising dozens of life-like tiger visuals in ecologically credible camera trap configurations paired with matching dermatoglyphic text descriptors of visible coat features. Benchmarking against real-world camera trap Re-ID scenarios shows that such augmentation can double AI accuracy in cross-modal retrieval while alleviating challenges of data scarcity for rare species and expert annotation bottlenecks. We conclude that dermatoglyphic language-guided animal biometrics can overcome key limitations of vision-only solutions and, for the first time, enable textual-to-visual identity recovery underpinned by human-verifiable minutiae matchings. Conceptually, this represents a significant advance towards explainability in Re-ID and a broader language-driven unification of descriptive modalities in AI-based ecological monitoring.



#### **From Visual Minutiae Features to Dermatoglyphic Text Descriptions**

Topological definitions of four common dermatoglyphic structural details (i.e. minutiae) are shown at the bottom left, with examples of these precise structures within a fingerprint to their right, as routinely determined during  forensic analysis. Above to the left, corresponding stripe arrangements are displayed on a synthesised tiger coat pattern. Following arrows to the right, the principles of the fingerprint ACE process are illustrated. Minutiae are identified along anatomically informed scan paths, sequentially encoded, and transformed into structured textual form. The resulting text is precisely interpretable, manually checkable against the visual, and at the same time compactly captures the individuality of the encoded pattern. This enables both `white box' matching and compact descriptor assembly across pattern categories beyond the scope of traditional computer vision-only models.

![](assets/media/images/minutiae.jpg)

#### **Visual-textual Co-Synthesis of Virtual Animal Coats**

Utilising spatial statistics of minutiae types is real anatomical pattern distributions across a population, we assemble full stripe textures based on a large minutiae library. The latter is constructed through keypoint augmentation, from which region-specific instances are sampled. ACE descriptors and language descriptions are paired with their expression in full-stripe textures to, once rendered, represent a virtual individual multi-modally. This forms the basis for producing any number of virtually rendered animal individuals simulating camera trap scenarios in order to produce realistic imagery for cross-modal AI training.

![](assets/media/images/statistical_synthesis.jpg)

#### **Distortion-corrected Texture Mapping and 3D Pose Modelling**

(a): Texture distortion caused by non-linear UV projections is corrected using RBF approximation, preserving anatomical consistency of the pelage pattern. (b): A controllable skeletal system with region-specific bindings enables natural 3D pose modelling by adjusting joints according to camera trap references. Examples of resulting animal poses that are realistically observable in real-world camera trap settings are shown on the right.

![](assets/media/images/rbf.jpg)


#### **Biomimetic Pelage Synthesis**

Anatomically-driven guides on the model surface are segmented by hair length~(short, medium, long) across anatomical regions; fur is generated along these guides, with pelage shapes driven by orientation and length parameters, and physical simulations achieved through perturbation, clumping, and frizz. The resulting fur textures~(right) have high fidelity and reduce any semantic gap to real population photography otherwise impeding on network training.

![](assets/media/images/hair.jpg)


#### **Visual Synthesis of Camera Trap Images of Virtual Tiger Identities.**

(a): Where current model-free AI synthesis would struggle to generate virtual individuals with truly matching image-text pairs, our automated virtual image construction pipeline produces pattern-consistent visualisations of life-like (virtual) tigers in camera trap scenarios. Virtual cameras capture 3D animal meshes with distinct coat pattern identity from multiple, task-specific angles under realistic HDRI lighting, with backgrounds from real camera trap images, and {are} post-processed via harmonisation and augmentation, mimicking field conditions {to reduce} the semantic gap to real-world imagery. (b): 24 samples within resolution range 301x156 to 413x195 from the 24,000 resulting multi-view animal renderings used for system training labelled with corresponding virtual animal IDs and exemplifying variations in real-world illumination and viewpoints akin to camera trapping. Note that identities are assigned -- as in field protocols in use -- to single sides (left or right) of the tiger. The reader may confirm virtual identities themselves to experience the difficulty of Re-ID from images for the species at hand.

![](assets/media/images/render.jpg)




---

### **Citation**

```BibTeX
@article{li2025visual,
  title={Visual-textual Dermatoglyphic Animal Biometrics: A First Case Study on Panthera tigris},
  author={Li, Wenshuo and Mirmehdi, Majid and Burghardt, Tilo},
  journal={arXiv preprint arXiv:2512.14878},
  year={2025}
}
 ```
---










