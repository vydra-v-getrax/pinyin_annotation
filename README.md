# pinyin_annotation
Repository for paper 'Comparative Analysis of Grapheme-to-Phoneme Models for the Russian-Chinese Parallel Corpus'. 


The Russian-Chinese parallel corpus of Ruscorpora (henceforth — the Corpus) is an online
corpus of texts, provided with linguistic markup and meta-information. The Corpus contains 1070
text samples of literary works, news, and others. So far, it lacks the proper annotation of pinyin
(Chinese transcription). Now the Grapheme-to-Phoneme (G2P) model applied to the Corpus is
based on the dictionary CEDICT [5]. Thus, all the possible transcriptions are ascribed to each
character without disambiguation. Therefore, the purpose of this study is to compare six G2P
models to improve the quality of pinyin markup of the Corpus. Chinese G2P conversion seems to
be challenging because of homophones and polyphones, which means that a character may have
multiple pronunciations. Besides, the Chinese texts in the Corpus contain many phonetic
borrowings from Russian which commonly are not included in dictionaries.

Tools explored:
* [A Context-aware Grapheme-to-Phoneme for Chinese](https://github.com/Kyubyong/g2pC) (G2pC) (2019)
* [A Neural Grapheme-to-Phoneme Conversion Package for Mandarin
Chinese Based on a New Open Benchmark Dataset](https://github.com/kakaobrain/g2pM) (G2pM) (2020)
* [xpinyin](https://github.com/lxneng/xpinyin)
(2002)
* [Chinese
Pinyin Conversion Tool for Python](https://github.com/mozillazg/python-pinyin) (pypinyin)

Jupyter notebook 'models tests.ipynb' runs models on human-annotated test dataset from the Russian-Chinese parallel corpus. 
G2pC model with additional pos-taggers runs automatically. To run tests on G2pM, xpinyin and pypinyin models, you need to pre-install them from the original source.


To original package [g2pC](https://github.com/Kyubyong/g2pC) were added FastHan and UDPipe POS-taggers. 

