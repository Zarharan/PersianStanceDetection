# Persian Stance Classification

We released here a Persian dataset that can be used for a number of NLP tasks in the context of fact-checking. Although this dataset can be used for fact-checking and summarization, the focus of this work is on stance classification as a stepping stone for fake news detection in the Persian language.

In order to collect this dataset, after collecting articles, for each claim we allocate three labels; the first label is article (body text) stance according to the claim (article-claim stance), the second label is the article’s headline stance according to the claim (headline-claim stance) and the third one is article (body text) stance according to its headline (article-headline stance). We release here article-claim stance as ArticleToClaim.txt file and headline-claim stance as HeadlineToClaim.txt file. In addition, we have released FullDataset.txt, this dataset can be used in order to stance detection and fake or rumor detection in Persian.

## Note
With respect to text embedding, we created matrix embeddings by using [fastText](https://dl.fbaipublicfiles.com/fasttext/vectors-crawl/cc.fa.300.bin.gz) and the <span style="color: green"> *create_embedding_matrix* </span> function in the <span style="color: green"> *LSTMPersianStance_HeadToClaim.ipynb* </span> file and saved this dictionary (matrix embedding) as <span style="color: green"> *w2v_persian.pkl* </span>. The matrix embedding is then loaded whenever it is needed.

We prepared a guideline in both English and Persian language, which consists of notes, suggestions, and examples about stance labels. The file named GuidLine_FA.pdf contains a Persian guideline and the file named GuideLine_EN.pdf contains an English guideline.

## The Dataset License 

Our Persian stance classification dataset is being provided to you under license CC BY-NC. You can read more about this licence [here](https://creativecommons.org/licenses/by-nc/4.0).

## The Related Paper

Our academic paper which describes the process of building our dataset in detail and provides full results can be found here: https://truthandtrustonline.files.wordpress.com/2019/10/paper_30.pdf .
