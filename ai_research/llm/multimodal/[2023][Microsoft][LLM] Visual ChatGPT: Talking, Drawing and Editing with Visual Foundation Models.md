# [2023][Microsoft][LLM] Visual ChatGPT: Talking, Drawing and Editing with Visual Foundation Models

- [arxiv](https://arxiv.org/pdf/2303.04671.pdf)
- [github](https://github.com/microsoft/visual-chatgpt)
----
## Introduction

A system called **Visual ChatGPT**, it is based on chatGPT and multiple **Visual Foundation Models(VFM)**.

### Needs
- It would consume a lot if data / computaitonal resources to build a multi-modality model every time.
- Current GPT3 is only support lanugage

### Proposed
- ChatGPT and VFMs

- ChatGPT engine
    - Open AI GPT3 `text-danvinci-003`
- Prompt Manager
    - Tell chatGPT each VFM and the input/output format
    - Convert different visual information to language
    - Handle the history
    - Tools
        - [langchain](https://github.com/hwchase17/langchain): A library help build applications with LLMs through composability 
- Support 22 VFMs at this research
    - [BLIP](https://huggingface.co/docs/transformers/model_doc/blip): provide visual QA/ Image-text retrievel/ Image Captioning
    - [Stable Diffusion](https://huggingface.co/docs/diffusers/stable_diffusion)
    - [MaskFormer](https://github.com/facebookresearch/MaskFormer): Meta's Semantic Segmentation
    - [ControlNet](https://github.com/lllyasviel/ControlNet): Let you control diffusion models

    - Detection
- Inference Requirements
    - 4 Nvidia V100GPU
    - Maximum length of chat: 2,000
- Limitations
    - Heavy prompt engineering
    - Limited Real-time Capabilities

## Architectute
![](https://i.imgur.com/ZPbkqx4.png)

## Overview
![](https://i.imgur.com/sS0ISdF.jpg)
