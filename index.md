---
layout: default
---

# Links

[Go to Project](https://jjong84.github.io/HowSample)

[Go to Google Colab Code](https://colab.research.google.com/drive/1B5A8QaD72YDuE8PHFNWZ3uCfZrzJbSHJ?usp=sharing)

[Go to Github Repository](https://github.com/JJong84/HowSample)

# Introduction

Sampling has become one of the most important composition techniques in modern music production. Numerous masterpiece tracks have been born through sampling, and many producers learn and get inspirations from understanding how these tracks were created and identifying their original sources. The best way to train and improve sampling skills is experiencing these breakdowns.

One representative database created by listeners' collective efforts is **“WhoSampled”**. It's a website that users can easily check which songs have sampled other tracks. However, it is hard to understand the specific sampling process because this site only provides basic song information. Additionally, users must breakdown the process by their own ears. And the descriptions are often inconsistent and unclear since it’s user-contributed.

Our web application, **“HowSample”** can be a great solution for these problems. It offers two modes, **breakdown mode** and **sampler mode**.

## Breakdown Mode

Breakdown mode, a powerful feature that analyzes the detailed sampling process of a track. The second is the Sampler mode which works similar to hardware sampler instruments. Users can load, edit, and apply effects to samples directly in the web interface to compose their own music. Moreover, samples analyzed in the breakdown mode can be directly loaded and used.

The Breakdown mode takes two inputs: the **target song** to be analyzed and the **original sampled song**. You can easily upload them by pressing **“SELECT TARGET AUDIO FILE”**, **“SELECT ORIGINAL AUDIO FILE”** buttons. Then, the uploaded song will be sent to the server and the breakdown result is sent back to the web. However, this feature is not implemented since our algorithm was not generalized yet.

Our goal was to focus on tracks produced through **time-stretching** and **pitch-shifting** processes. “HowSample” can automatically analyze and return the time-stretch factor and pitch-shift factor that is used in the detailed sampling process, also indicating the exact sections where sampling occurred.

You can check the demo by pressing the **“LOAD DEMO”** button. For the demo, we analyzed the target song **‘Kanye West – Through the Wire (2003)’**, which sampled **‘Chaka Khan – Through the Fire (1985)’**.

For the every waveforms in the breakdown result, you can easily click them to play them. The waveform shown at the top is the waveform of the **target song**. And the **blue colored part** is the analyzed segment. The analyzed segment is also shown as the **red colored waveform** below. The **green waveform** shows the sampled part of the target song. Its detailed time information is written at right side. Also, there are **time-stretch / pitch-shift information** too. By applying these effects with the analyzed factors, we can earn the blue waveform. You can check that the reproduced sample segment matches well with the target song. Also, you can check the analyzed samples are automatically loaded to the library at the sampler mode too.

The specific Breakdown process is explained at the following link:

[Goole Colab Link](https://colab.research.google.com/drive/1B5A8QaD72YDuE8PHFNWZ3uCfZrzJbSHJ?usp=sharing)

## Reference

Rouard, Simon, Francisco Massa, and Alexandre Défossez. **"Hybrid transformers for music source separation."**  
_ICASSP 2023-2023 IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP)._ IEEE, 2023.

Kim, Taejun, and Juhan Nam. **"All-in-one metrical and functional structure analysis with neighborhood attentions on demixed audio."**  
_2023 IEEE Workshop on Applications of Signal Processing to Audio and Acoustics (WASPAA)._ IEEE, 2023.
