# Graph2Seq
Graph2Seq model for English-to-Amharic machine translation, leveraging a syntax-directed tree structure of the source language to enhance translation quality. This approach integrates a dependency-based graph representation of English sentences, capturing syntactic and semantic relationships that guide the translation process.

Requirements
---------
```bash
    pip install tensorboard
    pip install torch==2.0.1 torchtext==0.15.2
```
How to run
----------

#### Start the StanfordCoreNLP server for data preprocessing:
1) Download dataset 'https://figshare.com/s/ce24e838cd0a142ca235'
2) Paste the row data to '/nmt/data'
3) Download StanfordCoreNLP `https://stanfordnlp.github.io/CoreNLP/`
4) Go to the root folder and start the server:

```java
    java -mx4g -cp "*" edu.stanford.nlp.pipeline.StanfordCoreNLPServer -port 9000 -timeout 15000
```


#### run script
``` bash
python nmt/main.py --name test
