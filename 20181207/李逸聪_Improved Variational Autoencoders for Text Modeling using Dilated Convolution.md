### ������Ŀ
Improved Variational Autoencoders for Text Modeling using Dilated Convolutions

### ����
Zichao Yang, Zhiting Hu, Ruslan Salakhutdinov, Taylor Berg-Kirkpatrick

Carnegie Mellon University

ICML 2017

###  ժҪ
Recent work on generative text modeling has found that variational autoencoders (VAE) with LSTM decoders perform worse than simpler LSTM language models (Bowman et al., 2015). This negative result is so far poorly understood, but has been attributed to the propensity of LSTM decoders to ignore conditioning informa- tion from the encoder. In this paper, we ex- periment with a new type of decoder for VAE: a dilated CNN. By changing the decoder��s di- lation architecture, we control the size of con- text from previously generated words. In ex- periments, we find that there is a trade-off be- tween contextual capacity of the decoder and ef- fective use of encoding information. We show that when carefully managed, VAEs can outper- form LSTM language models. We demonstrate perplexity gains on two datasets, representing the first positive language modeling result with VAE. Further, we conduct an in-depth investigation of the use of VAE (with our new decoding archi- tecture) for semi-supervised and unsupervised la- beling tasks, demonstrating gains over several strong baselines.

### �Ƽ�����
���Ƿ�����ICML 2017�ϵ�һƪ���¡�������Ҫ��������dilated CNN��Ϊ��ͳ��VAE�Ľ�������
���ڼ������ݼ���Ӧ���ˣ���LSTM����ģ��Ч���ã���������Ϊ2015��Bowman���˷��֣���
LSTM��Ϊ��������Ч����LSTM����ģ�Ͳ�����ڱ������������Ϊ�Ƚ϶��󣩡�

���⣬���߻����������϶԰�ල�Լ��޼ල��������ʵ�顣

### ���ĵ�ַ
[PDF ����](http://proceedings.mlr.press/v70/yang17d/yang17d.pdf)