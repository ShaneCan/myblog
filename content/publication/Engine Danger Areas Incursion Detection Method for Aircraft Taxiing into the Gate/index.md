---
abstract: Operational safety at airports has long been a subject of active research, with a growing focus on the safety of aircraft stands in recent years. The phase during which an aircraft taxi into its designated stand with engines still running poses safety risks to surrounding vehicles. However, there is currently a lack of effective methods for detecting potential conflicts and hazards during this taxiing phase. To address this issue, this study utilizes apron activity videos as a monitoring data source and introduces an integrated Internet of Things (IoT) conflict detection model. This system combines object detection, engine keypoint detection, coordinate conversion, and conflict warning system to provide timely alerts when vehicles incursion into the engine danger areas. Firstly, the paper streamlines the fourth-level branch and network of HRNet, resulting in the HRNet-3stage network. This network is then compared with Lite-HRNet to determine the optimal choice. Secondly, Recognizing the limitations of traditional video conflict detection based on pixel distance, a fixed monitoring camera coordinate conversion algorithm is designed to convert pixel coordinates into actual coordinates on the aircraft stand, thereby improving the accuracy of conflict detection based on distance measurement. Thirdly, considering the risks associated with engine inlet and exhaust, engine design parameters, static spacing standards, and the dynamic anti-collision process within the aircraft stand, the study proposes a method for classifying four types of aircraft engine danger areas. Corresponding conflict detection models are designed for potential scraping incidents when vehicles incursion into these danger areas. Upon detecting a vehicle entering the aircraft engine danger areas, the IoT system sends warning messages through the airport control tower monitoring system. Finally, we construct an apron sandbox to validate the conflict detection model. This validation results in an impressive F1-score exceeding 90% and a detection delay of less than 100ms. Our innovative approach, supported by keypoint detection networks and IoT, effectively addresses the detection of critical aircraft components within stands. It comprehensively analyzes incursion issues into engine danger areas, offering a novel perspective for understanding and mitigating potential conflicts arising from aircraft taxiing into stands.
# author_notes:
# - Equal contribution
# - Equal contribution
authors:
- Tianxiong Zhang
- Zhiqiang Zhang
- Xinping Zhu
- Honghao Chen
- Jiajun Li
- Yuming Zhong
date: "2024-03-13"
doi: "https://doi.org/10.1016/j.aej.2024.03.003"
featured: false
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/jdD8gXaTZsc)'
  focal_point: ""
  preview_only: false
projects: []
publication: 'Alexandria Engineering Journal'
publication_short: ""
publication_types:
- "2"
publishDate: "2024-03-13"
slides: Aircraft engine danger areas incursion detection using keypoint detection and IoT
summary: To mitigate the risk of irreversible damage caused by aircraft engines to equipment and personnel, addressing the scarcity of research on visualizing engine danger zones and conflict prevention.
tags:
- Source Themes
title: Aircraft engine danger areas incursion detection using keypoint detection and IoT
# url_code: https://github.com/wowchemy/wowchemy-hugo-themes
# url_dataset: ""
url_pdf: https://www.sciencedirect.com/science/article/pii/S1110016824002205
# url_poster: ""
# url_project: ""
# url_slides: ""
# url_source: ""
# url_video: ""
---


