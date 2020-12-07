---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "T-GCN: A Temporal Graph Convolutional Network for Traffic Prediction"
authors: [赵玲, 宋玉娇]
date: 2019-09-07T23:04:18+08:00
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: 2020-12-07T23:04:18+08:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: "T-GCN: A Temporal Graph Convolutional Network for Traffic Prediction"
publication_short: "T-GCN"

abstract: "准确、实时的交通预测在智能交通系统中发挥着重要作用，对城市交通规划、交通管理和交通控制具有重要意义。但由于受城市路网拓扑结构和随时间动态变化规律的限制，即空间依赖性和时间依赖性，交通预测一直被认为是一个开放的科学问题。为了同时捕捉空间依赖性和时间依赖性，我们提出了一种新型的基于神经网络的交通预测方法，即图卷积网络（GCN）和门控递归单元（GRU）相结合的时间图卷积网络（T-GCN）模型。具体来说，GCN用于学习复杂的拓扑结构以捕捉空间依赖性，门控递归单元用于学习流量数据的动态变化以捕捉时间依赖性。然后，采用T-GCN模型进行基于城市路网的交通预测。实验表明，我们的T-GCN模型可以从交通数据中获得时空相关性，并且在实际交通数据集上的预测结果优于最新的基线。我们的T-GCN的tensorflow实现见https://github.com/lehaifeng/T-GCN。"

# Summary. An optional shortened abstract.
summary: ""

tags: []
categories: []
featured: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_pdf: publication/TGCN/paper.pdf
url_code:
url_dataset:
url_poster:
url_project: https://github.com/lehaifeng/T-GCN
url_slides:
url_source:
url_video:

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---
本文提出了一种基于神经网络的新型交通预测方法，称为T-GCN，它结合了GCN和GRU。我们采用图网络对城市道路网进行建模，图上的节点代表道路，边代表道路之间的连接关系，道路上的交通信息被描述为图上节点的属性。一方面，利用GCN捕捉图的拓扑结构，得到空间上的依赖性；另一方面，利用GRU模型捕捉节点属性的动态变化，得到时间上的依赖性。最终采用T-GCN模型来解决时空交通预测任务。在两个真实世界的交通数据集上进行评估，并与HA模型、ARIMA模型、SVR模型、GCN模型和GRU模型进行比较，T-GCN模型在不同的预测视野下取得了最好的预测效果。此外，扰动分析也说明了我们方法的稳健性。综上所述，T-GCN模型可以成功-充分捕捉交通数据的时空特征，并且不局限于交通预测，还可以应用于其他时空任务。