---
abstract: To address the problems of poor level of detail in existing aircraft detection models, limited types of conflict recognition on aprons, and simplified safety zone settings which cannot meet the safety monitoring needs of air traffic controllers, a multi-keypoint detection method for detecting conflicts between aircraft and apron moving vehicles during the aircraft taxi-in process and in the apron parking state is proposed. The proposed method uses a high-resolution keypoint detection network, HRNet, to identify key components such as the nose, engine, and wingtip in a dynamic and refined way. The apron surveillance video is used as the data source, and coordinate conversion algorithm is designed to convert image pixel coordinates to the actual coordinates of the apron surface, improving the accuracy of conflict determination. Kinematic characteristics of aircraft and vehicles in the apron are considered, and an aircraft taxi-in deceleration model and a service vehicle movement model are established. The method includes a safety zone designation approach for aircraft and vehicles in the apron based on apron operation control rules. A multiple conflict detection strategy is designed to address the concurrent occurrence of various conflicts and enable parallel processing of multiple conflicts. A physical sandbox is constructed to compare and analyze the selected aircraft keypoint detection network, and eight typical conflict scenarios are designed to validate the proposed method through simulation experiments. The results show that the keypoint network outperforms the mainstream keypoint detection network in apron operation scenarios. The proposed method achieves real-time aircraft multi-component conflict monitoring, compared with the single-component-based aircraft conflict detection method. The conflict detection method that is designed possesses a high level of accuracy and timeliness, with an Average Precision rate of 96.82 %, an Average Recall rate of 94.87 %, and a calculation delay of 311 ms. The proposed method can provide a reliable means to discriminate and prevent conflicts between aircraft and apron vehicles.
# author_notes:
# - Equal contribution
# - Equal contribution
authors:
- Tianxiong Zhang
- Zhiqiang Zhang
- Xinping Zhu
- Jiajun Li

date: "2023-03-01T00:00:00Z"
doi: ""
featured: false
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/jdD8gXaTZsc)'
  focal_point: ""
  preview_only: false
projects: []
publication: 'Journal of Transport Information and Safety'
publication_short: ""
publication_types:
- "2"
publishDate: "2023-06-01T00:00:00Z"
slides: A Multi-Keypoint Detection Based Method for Conflict Determination between Aircraft and Vehicles on the Apron Gate
summary: Use CV to solve Apron safety problem.
tags:
- Source Themes
title: A Multi-Keypoint Detection Based Method for Conflict Determination between Aircraft and Vehicles on the Apron Gate
# url_code: https://github.com/wowchemy/wowchemy-hugo-themes
# url_dataset: ""
# url_pdf: https://ietresearch.onlinelibrary.wiley.com/doi/epdf/10.1049/itr2.12314
# url_poster: ""
# url_project: ""
# url_slides: ""
# url_source: ""
# url_video: ""
---


