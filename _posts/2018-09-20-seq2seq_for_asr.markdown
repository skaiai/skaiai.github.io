---
layout: post
title: "Sequence-to-Sequence Models for ASR (1)"
tags: seq2seq speech-recognition
categories: speech-recognition
comments: true
---
<!--last update: 2018-09-20 <br/><br/>-->

last update: 2018-09-26<br/>
Next Post: [Sequcne-to-Sequence models for ASR (2): Transformer for ASR]({{ site.baseurl }}/speech-recognition/2018/09/26/transformer_for_asr.html)

---
<!-- > End-to-end approach to speech recognition is appealing to us, as it turns separate models such as AM (acoustic), PM (pronunciation), LM (language) of conventional hybrid ASR system into one single neural network model.<br/><br/>Seq-to-seq models have been used for this purpose and I'd like to review them.<br/> -->

End-to-end approach to speech recognition is appealing to us, as it turns separate models such as AM (acoustic), PM (pronunciation), LM (language) of conventional hybrid ASR system into one single neural network model.<br/>

Seq-to-seq models have been used for this purpose and I'd like to review them.<br/>

---
## Seq2Seq Models
#### 1. Connectionist temporal classification (**CTC**)
* [Connectionist Temporal Classification: Labelling Unsegmented Sequence Data with Recurrent Neural Networks](https://www.cs.toronto.edu/~graves/icml_2006.pdf) 
* when: 2006 by Alex Graves

#### 2. Recurrent neural netowrk Transducer (**RNN-T**)
* [Sequence transduction with recurrent neural networks](https://arxiv.org/pdf/1211.3711.pdf) 
* when: Nov 2012 by Alex Graves
* description: extension of CTC (it augments CTC w/ prediction network)

#### 3. Attention-based Model
* **LAS** model (non-streaming input)
	* [Listen, Attend and Spell](https://arxiv.org/pdf/1508.01211.pdf) 
	* when: Aug 2015 by CMU, Google Brain
	* description: encoder, decoder and attention btw them. non-streaming input
* **Nueral Transducer** (streaming input)
	* improved: [Improving the performance of online neural transducer models](https://pdfs.semanticscholar.org/9409/ce44b3c6b1b55479f3ff0f87f4e7c52f227a.pdf)
		* Dec 2017 by Google
	* org: [An online sequence-to-sequence model using partial conditioning](http://bengio.abracadoudou.com/cv/publications/pdf/jaitly_2016_nips.pdf)
		* when: 2016 by Google Brain / DeepMind, OpenAI
		* description: streaming input

#### 4. **RNN-T w/ Attention**
* [A comparison of sequence-to-sequence models for speech recognition](https://pdfs.semanticscholar.org/6cc6/8e8adf34b580f3f37d1bd267ee701974edde.pdf)
* 2017 by Google, NVIDIA
* description: modification to the RNN transducer replacing the prediction network w/ attention-based decoder entwork used in LAS

#### 5. **Transformer**
* [Attention is all you need](https://papers.nips.cc/paper/7181-attention-is-all-you-need.pdf)
* 2017 by Google Brain/Research, University of Toronto
* description: attention operations are introduced in encoder and decoder nets both instead of rnn or cnn

---
Next post will be discussing Transformer model and how to apply it to ASR task.
