# [2022][JHU] SELF-INSTRUCT: Aligning Language Model with Self Generated Instructions

- arxiv: https://arxiv.org/pdf/2212.10560.pdf
- code: https://github.com/yizhongw/self-instruct


![](https://i.imgur.com/zUE1Ya0.png)

## Intro
- A framework for improving a language model by its own generations
    - following by minimal human-labeled data `52K` instructions

- Language models for data generation and augmentation
- A model's knowledge is distilled to itself


## Method

1. Define the instruction data
2. Automatic Instruction Data Generation
    a. Instruction Generation
    b. classification task identification 
    c. Instance generation
    d. Use different template to combine the instruction and instance, ex: Task:/ Input: / Output:
    
## Discussion and Limitation
1. Why does self-instruct work?
    - human feedback is a necessary and indispensable
    - human feedback is an optional aspect of instruction tuning as LMs are already quite familiar with instructions 

- Limitations
    - LMs’ largest gains correspond to the frequent uses of languages (head of the language use distribution), and there are min-imal gains in the low-frequency contexts.
    - SELF-INSTRUCT’s dependence on the inductive biases extracted from LMs, it might work best for larger models

## Related 
- [2023][Standford]Alpaca: A Strong Open-Source Instruction-Following Model
    - https://crfm.stanford.edu/2023/03/13/alpaca.html
    - demo: https://crfm.stanford.edu/alpaca/

![](https://i.imgur.com/UW04ZN1.png)
