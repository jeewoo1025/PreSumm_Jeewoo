# PreSumm_Jeewoo
The origin project is [PreSumm](https://github.com/nlpyang/PreSumm). I modified codes of this project because the version of PyTorch is different and I suit my development environment.

* origin paper : [Text Summarization with Pretrained Encoders](https://arxiv.org/abs/1908.08345) (EMNLP, 2019)
* [PreSumm](https://github.com/nlpyang/PreSumm) PyTorch version : 1.1.0, My Pytorch version : 1.11.0

<br>

Results on CNN/DailyMail (2022.04.05):
|Models|ROUGE-1|ROUGE-2|ROUGE-L|
|:---:|:---:|:---:|:---:|
|BertSumExt|42.89|20.09|39.33|
|BertSumAbs|41.23|18.86|38.27|

<br>

Results on XSum (2022.04.07):
|Models|ROUGE-1|ROUGE-2|ROUGE-L|
|:---:|:---:|:---:|:---:|
|BertSumExt|21.74|4.27|16.99|

<br>

<strong>Python version</strong> : This code is in Python 3.8 <br>
<strong>PyTorch version</strong> : This code is in PyTorch 1.11.0 <br>

<br>

## Note
The only difference from the origin project is the `/src`. So, please make directories as follows. 
* `/bert_data`
* `/models`
* `/logs`
* `/results`

<br>

## Example summary from BertSum models
### CNN/DailyMail
The input document and gold summary are randomly picked from CNN/DailyMail testset. The sentences in red are extracted by the BertSumExt, and the sentences in green are similar to the generated summary of BertSumAbs. 
![CNNDM_요약문](https://user-images.githubusercontent.com/39071676/161654697-80133096-ffa2-4086-95b0-78b095ac026b.png)
I find the summary of BertSumAbs tends to copy sentences from input documents. CNN/DailyMail dataset has extractive characteristics, so this phenomenon occurs when this model is fine-tuned with this dataset.
