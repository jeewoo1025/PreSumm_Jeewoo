# PreSumm_Jeewoo
The origin code is [PreSumm](https://github.com/nlpyang/PreSumm). I modified codes of this project because the version of PyTorch is different and I suit my development environment.

* origin paper : [Text Summarization with Pretrained Encoders](https://arxiv.org/abs/1908.08345) (EMNLP, 2019)
* [PreSumm](https://github.com/nlpyang/PreSumm) PyTorch version : 1.1.0, My Pytorch version : 1.11.0

<br>

Results on CNN/DailyMail (2022.04.05):
|Models|ROUGE-1|ROUGE-2|ROUGE-3|
|:---:|:---:|:---:|:---:|
|BertSumExt|42.89|20.09|39.33|
|BertSumAbs|41.23|18.86|38.27|

<strong>Python version</strong> : This code is in Python3.8 <br>
<strong>PyTorch version</strong> : This code is in PyTorch 1.11.0 <br>

## Note
The only difference from the origin project is the `\src`. So, please make diretories as follows. 
* `/bert_data`
* `/models`
* `/logs`
* `/results`
