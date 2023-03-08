# [2023][Microsoft][TTS]Speak Foreign Languages with Your Own Voice:Cross-Lingual Neural Codec Language Modeling

- [arxiv](https://arxiv.org/pdf/2303.03926.pdf)
- [github](https://github.com/microsoft/unilm)

![](https://i.imgur.com/1kKJc9q.png)


## Intro

- A cross-lingual neural codec language model, VALL-EX
- A comparison between VALL-E X and previoud cross-lingual TTS systems
![](https://i.imgur.com/hPCUCTA.png)
- It's conditional cross-lingual language model 
    - input: source language speech/ target language text
    - output: target language token

- It is a `In-context learning framework`
    - [What is in-context learning?](http://ai.stanford.edu/blog/understanding-incontext/)
    >  LM does in-context learning by using the prompt to “locate” the relevant concept it has learned during pretraining to do the task. We can theoretically view this as Bayesian inference of a latent concept conditioned on the prompt, and this capability comes from structure (long-term coherence) in the pretraining data.


- Training illustration

![](https://i.imgur.com/QQqVLKB.png)

- Inference illustration
![](https://i.imgur.com/qU3bHMq.png)
- Compare to YouTTS(baseline)
- Add Language ID to guide the speech synthesis to avoid the accent score.

## Tools
- Convert transcript to phoneme sequence: [G2P Tool](https://github.com/Kyubyong/g2p)
- Convert speech into discrete codec codes as the acoustic tokens with the neural audio codec [EnCodec](https://github.com/facebookresearch/encodec)
