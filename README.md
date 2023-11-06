# KoPolitic-Benchmark-Dataset
## A New Korean Text Classification Benchmark for Recognizing the Politic Intents in Online Newspapers
- This repository provides **KoPolitic Dataset** and PyTorch implementations for classification models<br>(**KoPolitic**, KoBigBird, KoBERT, KoELECTRA).

## Authors
- [Beomjune Kim](https://github.com/Kdavid2355), [Eunsun Lee](https://github.com/eunsun111), [Dongbin Na](https://github.com/ndb796)

## Abstract

>Many users reading online articles in various magazines may suffer considerable difficulty in distinguishing the implicit intents in texts.
In this work, we focus on automatically recognizing the political intents of a given online newspaper by understanding the intent of the text. To solve this task, we present a novel Korean text classification dataset that contains various articles. We also provide deep-learning-based text classification baseline models trained on the proposed dataset.
Our dataset contains 12,000 news articles that may contain political intentions, from the \textit{politics} section of six of the most representative newspaper organizations in South Korea.
All the text samples are labeled simultaneously in two aspects (1) the level of political orientation and (2) the level of pro-government.
To the best of our knowledge, our paper is the most large-scale Korean news dataset that contains long text and addresses multi-task classification problems. We also train recent state-of-the-art (SOTA) language models that are based on transformer architectures and demonstrate that the trained models show decent text classification performance. All the source codes, datasets, and trained text classification models will be publicly available after our paper is accepted.

## Model
- The conceptual illustration of our model with input and output examples.

![KakaoTalk_Photo_2023-10-17-22-12-14](https://github.com/Kdavid2355/KoPolitic-Benchmark-Dataset/assets/50067299/5101b14b-5cb3-4cbe-bc39-3cb3e6070c13)

## Source Codes

| Model       | SeqLen | Code       |
|:------------------:|:-------:|------------|
| KoBigBird   | 1024  | [link1](링크1_URL) |
| KoBigBird   | 2048  | [link2](링크2_URL) |
| KoBigBird   | 3072  | [link3](링크3_URL) |
| KoPolitic   | 1024  | [link4](링크4_URL) |
| KoPolitic   | 2048  | [link5](링크5_URL) |
| KoPolitic (Ours)  | 3072  | [link6](링크6_URL) |
| Kobert Single    | 512 | [link7](링크7_URL) |
| Kobert Multi     | 512  | [link8](링크8_URL) |
| KoElectra Single | 512 | [link9](링크9_URL) |
| KoElectra Multi  | 512  | [link10](링크10_URL) |

## Models Performance
- The classification performance of trained model.

<img width="1101" alt="스크린샷 2023-10-17 오후 10 47 27" src="https://github.com/Kdavid2355/KoPolitic-Benchmark-Dataset/assets/50067299/f2271590-b07f-4262-889d-b72adc63e3b9">


## Dataset

The dataset consists of 12,000 news articles. Articles were crawled and collected from six leading newspapers in South Korea. This includes two newspapers classified as conservative, two as neutral, and two as liberal. Out of the 12,000 labeled articles, 5,000 of the dataset are labeled based on two criteria: the level of political orientation and the level of pro-government. The level of political orientation is rated on a 5-point scale, where a score closer to 1 indicates a liberal stance and a score closer to 5 indicates a conservative stance. The level of pro-government is rated on a 6-point scale, where 0 stands for ‘None', scores closer to 1 indicate support for the government, and scores closer to 5 indicate criticism of the government.

<p align="center">
  <img width="800" alt="이미지 설명" src="https://github.com/Kdavid2355/KoPolitic-Benchmark-Dataset/assets/50067299/fb73ddcf-ef9b-4b79-bdb4-ae9e39debb3f">
</p>


<p align="center">
  <img width="999" alt="스크린샷 2023-10-17 오후 10 42 14" src="https://github.com/Kdavid2355/KoPolitic-Benchmark-Dataset/assets/50067299/156f6789-3b9f-4e81-a15e-56b91cef4861">    
</p>

[Download Dataset](https://drive.google.com/drive/u/1/folders/1ru4mD3aHoFIc1w5r0xnEO27ntFEkZIUa)

## Citation 
If this work can be useful for your research, please cite our paper:


@misc{kim2023new, <br>
      title={A New Korean Text Classification Benchmark for Recognizing the Political Intents in Online Newspapers}, <br>
      author={Beomjune Kim and Eunsun Lee and Dongbin Na},      
      year={2023},      
      eprint={2311.01712},      
      archivePrefix={arXiv},      
      primaryClass={cs.CL} <br>
}
