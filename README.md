# Pytorch implementation of summarization with Pointer-Generator Networks.

An implementation of a paper ["Get To The Point: Summarization with Pointer-Generator Networks"](https://arxiv.org/pdf/1704.04368.pdf) with a few modifications added.

## Baseline scores comparison	

Evaluating on [ria-news](https://github.com/RossiyaSegodnya/ria_news_dataset) dataset.

Baseline\Metric | rouge-1-f	| rouge-1-p	| rouge-1-r	| rouge-2-f	| rouge-2-p	| rouge-2-r	| rouge-l-f	| rouge-l-p	| rouge-l-r |
--------- | --------- | --------- | --------- |  --------- | --------- | --------- | --------- | --------- | --------- |
First sentence | 0.10515622 | 0.08202730 | 0.17109826 |  0.02310585 | 0.01773702 | 0.04013821 | 0.07781251 | 0.07387972 | 0.15335960 |
Seq2seq+attn | 0.27272711 |	0.29711504 |	0.26069220 |	0.14079773 |	0.15397009 |	0.13496864 |	0.24934808 |	0.28070855 |	0.24599733 |
Pointer-Generator | 0.39365891 | 0.41640767 | 0.38165893  |0.22586564 | 0.23952421 |  0.21927996 | 0.36739665 | 0.39729979 |  0.36412255 |
Seq2seq+attn+glove | 0.40667004 | 0.42953731 | 0.39510796 | 0.23331091 | 0.24639854 | 0.22753361 | 0.37873374 | 0.40884524 |    0.37604734 |
Seq2seq+attn+w2v | 0.40642236 | 0.42634267 | 0.39755649 | 0.23379854 | 0.24523071 | 0.22947409 | 0.37832096  |  0.40559853 | 0.37798990 |
