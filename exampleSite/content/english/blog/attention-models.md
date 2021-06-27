+++
bg_image = "/images/mainlogo.png"
categories = ["NLP"]
date = 2021-06-20T18:30:00Z
description = "Attention"
draft = true
image = ""
tags = []
title = "Attention models"
type = "post"

+++
Attention models are the state of the art models in NLP.

This is sample blog.

> Attention is all you need

    import numpy as np
    import pandas as pd

Recurrent models typically factor computation along the symbol positions of the input and output sequences. Aligning the positions to steps in computation time, they generate a sequence of hidden states ht, as a function of the previous hidden state ht−1 and the input for position t. This inherently sequential nature precludes parallelization within training examples, which becomes critical at longer sequence lengths, as memory constraints limit batching across examples. Recent work has achieved significant improvements in computational efficiency through factorization tricks \[18\] and conditional computation \[26\], while also improving model performance in case of the latter. 

The fundamental constraint of sequential computation, however, remains. Attention mechanisms have become an integral part of compelling sequence modeling and transduction models in various tasks, allowing modeling of dependencies without regard to their distance in the input or output sequences \[2, 16\]. In all but a few cases \[22\], however, such attention mechanisms are used in conjunction with a recurrent network. 

In this work we propose the Transformer, a model architecture eschewing recurrence and instead relying entirely on an attention mechanism to draw global dependencies between input and output. The Transformer allows for significantly more parallelization and can reach a new state of the art in translation quality after being trained for as little as twelve hours on eight P100 GPUs.