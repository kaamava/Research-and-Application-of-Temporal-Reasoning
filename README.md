## Improving Temporal Generalization of Pre-trained Language Models with Lexical Semantic Change

This repository contains part of the code and pre-trained models for our paper "Awareness of Time: Video-Language Models Embedding with Temporal Reasoning", which has been submitted to LREC-COLING2024. The complete code will be released after the conference announces the acceptance results.

## Overview

- Overview
- Datasets
- Baseline
- Train
- Results


## Overview

·We show that existing video-language models have difficulty in associating time order in video and language through controlled experiments on synthetic data and several evaluations on real datasets.

·We propose a temporal reasoning video-language pre-training framework with both videolanguage understanding and generation capabilities.

·We introduce temporal reasoning pre-training tasks to generate temporal reasoning multi-modal representation through modeling fine-grained temporal moment information and capturing the temporal contextual relations between moment and event.


## Datasets

we pre-train our model on a webly-sourced video dataset WebVid-2M with 2.5M video-text pairs and a image-text dataset Google Conceptual Captions (CC3M) with 3M image-text pairs. Unlike previous methods, we do not pre-train our model on the large-scale video-text datasets like HowTo100M with 136M video-text pairs and YT-Temporal-180M due to the heavy computation.

![tempo-data-v1](https://github.com/kaamava/Research-and-Application-of-Temporal-Reasoning/assets/106901273/1bff9281-7ea3-4896-aadf-72dbfa49d396)


We evaluate our pre-trained model on several video-language benchmarks including video-text retrieval, video question answering, and video captioning tasks. Specifically, video question answering (VideoQA) can be categorized as Multiple-Choice (MC) and Open-Ended (OE) settings. The evaluation datasets are briefly summarized in below. 

• Video-Text Retrieval: MSRVTT, DiDeMo, LSMDC, ActivityNet Caption, and SSv2-Template;

• VideoQA (MC): TGIF-Action, TGIF-Transition, MSRVTT-MC, LSMDC-MC, and NExT-QA;

• VideoQA (OE): TGIF-Frame, MSRVTT-QA,MSVD-QA, LSMDC-FiB and ActivityNet-QA;

• Video Captioning: MSRVTT and MSVD.
## Baseline


| **Post-pretraining Dataset** 	|                        	|   **Hyperparameters**   	|         	| **Download link** 	|
|------------------------------	|:----------------------:	|:-----------------------:	|:-------:	|:-----------------:	|
|                              	| $\alpha_{\text{same}}$ 	| $\alpha_{\text{cross}}$ 	| $\beta$ 	|                   	|
| TEMPO-TL                     	|           1.0          	|           1.0           	|   1.0   	|        [Link](https://isis-data.science.uva.nl/testoftime/checkpoints/tempo-hparams_1.0_1.0_1.0-epoch=27-step=8288.ckpt)       	|
| ActivityNet                  	|           1.0          	|           1.0           	|   0.0   	|        [Link](https://isis-data.science.uva.nl/testoftime/checkpoints/activitynet-hparams_1.0_1.0_0.0-epoch%3D9-step%3D7450.ckpt)       	|
| Charades                     	|           1.0          	|           1.0           	|   0.0   	|        [Link](https://isis-data.science.uva.nl/testoftime/checkpoints/charades-hparams_1.0_1.0_0.0-epoch%3D3-step%3D3120.ckpt)       	|
| Charades-Ego                 	|           1.0          	|           1.0           	|   1.0   	|        [Link](https://isis-data.science.uva.nl/testoftime/checkpoints/charadesego-hparams_1.0_1.0_1.0-epoch%3D2-step%3D3639.ckpt)       	|

## Train
## Result
*These two parts will be released after the conference announces the acceptance results.*

