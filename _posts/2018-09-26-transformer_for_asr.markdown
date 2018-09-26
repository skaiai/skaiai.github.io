---
layout: post
title: "Sequence-to-Sequence Models for ASR (2): Transformer for ASR"
tags: seq2seq speech-recognition
categories: speech-recognition
comments: true
---
<!--last update: 2018-09-20 <br/><br/>-->

last update: 2018-09-26<br/>
Previous Post: [Sequcne-to-Sequence models for ASR (1)]({{ site.baseurl }}/speech-recognition/2018/09/20/seq2seq_for_asr.html)

---




Next post will be discussing Transformer model and how to apply it to ASR task.

End-to-end approach to speech recognition is appealing to us, as it turns separate models such as AM (acoustic), PM (pronunciation), LM (language) of conventional hybrid ASR system into one single neural network model.<br/>

Seq-to-seq models have been used for this purpose and I'd like to review them.<br/>

---

#### 5. **Transformer**
* [Attention is all you need](https://papers.nips.cc/paper/7181-attention-is-all-you-need.pdf)
* 2017 by Google Brain/Research, University of Toronto
* description: attention operations are introduced in encoder and decoder nets both instead of rnn or cnn

---
