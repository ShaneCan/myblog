---
abstract: Applications of Innovative Air Mobility (IAM) place high demands on the safe coordination of multiple UAVs and UAV-tailored takeoff and landing pads, to mitigate unforeseen adverse effects. However, existing modeling approaches for multi-UAV flight operation often provide neither formal correctness guarantees nor effective mechanisms for maintaining cyber–physical consistency. To address these limitations, this paper proposes a bigraph-based digital twin framework that unifies modeling, execution, and synchronization for the management of landing operations involving multiple UAVs. Leveraging Bigraphical Reactive Systems (BRS), the framework employs a Bigrid-based spatial model to formally represent UAV–pad occupancy constraints and to enforce one-to-one pad assignments via reaction rules, supporting formal proofs of safety properties. The model is linked to physical execution through modular APIs and a state-machine-based control service, enabling runtime cyber–physical synchronization. The formal specification is verified through model checking, which exhaustively explores the solution space (i.e., UAV behaviors in abstracted environments) to identify bigraph-algebraic solutions that guarantee conflict-free landings across different pad configurations. The framework is instantiated on the Crazyflie platform, demonstrating its ability to bridge formal modeling and physical execution while maintaining safety, scalability, and robustness in operational scenarios involving multiple UAVs.
# author_notes:
# - Equal contribution
# - Equal contribution
authors:
- Tianxiong Zhang
- Dominik Grzelak
- Martin Lindner
- Hartmut Fricke
- Uwe Aßmann
date: "2025-11-30"
# doi: "https://doi.org/10.3390/drones9060394"
featured: false
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/jdD8gXaTZsc)'
  focal_point: ""
  preview_only: false
projects: []
publication: 'Drones'
publication_short: ""
publication_types:
- "2"
# publishDate: "2025-05-24"
slides: Bigraph-based Digital Twin for Multi UAV Landing Management.
summary: A bigraph-based digital twin framework for coordinating safe multi-UAV landing operations in Innovative Air Mobility scenarios.
tags:
- Source Themes
title: Bigraph-based Digital Twin for Multi UAV Landing Management
# url_code: https://github.com/wowchemy/wowchemy-hugo-themes
# url_dataset: ""
# url_pdf: https://mdpi-res.com/d_attachment/drones/drones-09-00394/article_deploy/drones-09-00394.pdf?version=1748093258
# url_poster: ""
# url_project: ""
# url_slides: ""
# url_source: ""
# url_video: ""
---


