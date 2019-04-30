# Pytorch implementation of summarization with Pointer-Generator Networks.

An implementation of a paper "Get To The Point: Summarization with Pointer-Generator Networks" (https://arxiv.org/pdf/1704.04368.pdf) with a few modifications added.

## Baseline scores comparison	

Evaluating on ria-news dataset.

Baseline\Metric | rouge-1-f	| rouge-1-p	| rouge-1-r	| rouge-2-f	| rouge-2-p	| rouge-2-r	| rouge-l-f	| rouge-l-p	| rouge-l-r |
--------- | --------- | --------- | --------- |  --------- | --------- | --------- | --------- | --------- | --------- |
First sentence	| 0.10515622 | 0.08202730 | 0.17109826 |  0.02310585 | 0.01773702 | 0.04013821 | 0.07781251 | 0.07387972 | 0.15335960 |
Seq2seq+attn    | 0.13303332 | 0.15463217 | 0.12296674 | 0.04624813  | 0.05416022 | 0.04320243 | 0.11961113 | 0.14709123 | 0.11673100 |
