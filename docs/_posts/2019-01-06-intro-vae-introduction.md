---
title: IntroVAE:IntrospectiveVariationalAutoencodersfor PhotographicImageSynthesis
author: zhangruru1
comments: true
mathjax: true
categories: 
  - generative model
tags:
  - vae
---
Link: http://papers.nips.cc/paper/7291-introvae-introspective-variational-autoencoders-for-photographic-image-synthesis
   IntroVAE推理和生成器模型以一种内省的方式联合训练。一方面，需要生成器将推理模型的噪声输出重构为正常的VAE输入图像；另一方面，推理模型在生成的样本和实际样本之间进行分类，而生成器则试图将其伪装成GAN。IntroVAE保留了VAEs的优点，如训练稳定，潜在流形良好。与大多数其他混合的VAEs和GANs模型不同，IntroVAE不需要额外的判别器，因为推理模型本身就是一个判别器，用来区分生成的样本和真实样本。
IntroVAE架构和培训流程：
https://user-images.githubusercontent.com/40236999/58746892-5fe03200-8496-11e9-89e3-a9571e0390b6.png
训练过程：
https://user-images.githubusercontent.com/40236999/58746928-bd747e80-8496-11e9-85df-59090ad56770.png
结果表现：
https://user-images.githubusercontent.com/40236999/58746932-cb2a0400-8496-11e9-8a88-57855bc50186.png
