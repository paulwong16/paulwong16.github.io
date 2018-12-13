---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

- Xinjun Liu, Chao Yu, Fei Qiao, Fugui Xie, **Zhijie Wang**, A Robot SLAM System Towards Dynamic En-vironments, *CN Patent*. No. CN 108596974A. **Published** ([Download](http://paulwong16.github.io/files/2018102980426.pdf))

- Zelei Cheng, **Zhijie Wang**, Feng Zheng, Cloud Computing Security, *2018 International Conference on Trustworthy Computing and Services*. **Accpeted** ([Download]())

- Xiaodong Liu, **Zhijie Wang**, Yu Herng Tan, Yingcai Bi, Ben M. CHen, Underwater Image Enhancer based on Conditional GANs, *IEEE International Conference on Robotics and Automation 2019*. **Submitted**

- **Zhijie Wang**, Yingcai Bi, Ben M. Chen, Continuous Localization and Mapping for Autonomous Navigation in low-light environments based on Multi-Sensors Fusion, *IEEE International Conference on Control and Automation*. **Submitted**