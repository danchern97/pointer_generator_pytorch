# Pytorch implementation of summarization with Pointer-Generator Networks.

An implementation of a paper ["Get To The Point: Summarization with Pointer-Generator Networks"](https://arxiv.org/pdf/1704.04368.pdf) with a few modifications added.

## Baseline scores comparison	

Evaluating on [ria-news](https://github.com/RossiyaSegodnya/ria_news_dataset) dataset.

Baseline\Metric | rouge-1-f	| rouge-1-p	| rouge-1-r	| rouge-2-f	| rouge-2-p	| rouge-2-r	| rouge-l-f	| rouge-l-p	| rouge-l-r |
--------- | --------- | --------- | --------- |  --------- | --------- | --------- | --------- | --------- | --------- |
First sentence | 0.10515622 | 0.08202730 | 0.17109826 |  0.02310585 | 0.01773702 | 0.04013821 | 0.07781251 | 0.07387972 | 0.15335960 |
Seq2seq+attn | 0.41582201 | 0.43718827 | 0.40561483 | 0.24086001 |  0.25307833 | 0.23581065 | 0.38644251 | 0.41508011 | 0.38504612 |
Pointer-Generator | 0.41094998 | 0.43332178 | 0.39906258 | 0.24201008 | 0.25566738 | 0.23547465 | 0.38392726 | 0.41334106 | 0.38063485 |
Seq2seq+attn+glove | **0.41925908** | **0.44047456** | **0.40921883** | **0.24513830** | **0.25763531** | **0.23992956** | **0.39001231** | **0.41847043** | **0.38874970** |
Pointer-Generator+Glove | 0.41242970 | 0.43542033 | 0.40028182 | 0.24193624 | 0.25587737 | 0.23518939 | 0.38503439 | 0.41518183 | 0.38158816 |
Seq2Seq+attn+unsup | 0.27785800 | 0.29142466 | 0.27177418 | 0.13108816 | 0.13720493 | 0.12893772 | 0.25623700 | 0.27484959 | 0.25632151 |
Seq2Seq+attn+ner | 0.15539128 | 0.16671571 | 0.14977648 | 0.05272446 | 0.05646063 | 0.05105246 | 0.14240497 | 0.15737464 | 0.14127297 |
Seq2Seq+attn+1sent | 0.17119596 | 0.18658731 | 0.16277689 | 0.05889539 | 0.06410998 | 0.05628019 | 0.15706118 | 0.17683240 | 0.15422777 |
