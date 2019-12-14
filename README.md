**This is work in progress**

# Beto Benchmarks

The following table shows the BETO results in the Spanish version of every task/benchamrk with links to the
hyperparameter settings used in every experiment. 
We compare BETO (cased and uncased) with the Best Multilingual-BERT result that 
we found in the literature (as of October 2019) highlighting 
the results whenever BETO ourperform Multilingual BERT. 
The table also shows some alternative methods for the same tasks (not necessarily BERT-based methods).
References for all methods are included below.

|Task   | BETO-cased    | BETO-uncased  | Best Multilingual Bert    | Other results                  |
|-------|--------------:|--------------:|--------------------------:|-------------------------------:|
|XNLI   | -----         | [**80.15**](grid_search_XNLI.txt)  | 78.50 [2]| 80.80 [5], 77.80 [1], 73.15 [4]|
|POS    | -----         | [**98.44**](grid_search_POS.txt)   | 97.10 [2]| 98.91 [6], 96.71 [3]           |
|PAWS-X | -----         | [89.55](experiments_pawsx.txt) | 90.70 [8]|
|NER-C  | 86.58         | 81.70                          | 87.38 [2]| 87.18 [3]                      |
|NER-W  | -----         | -----                          | 92.50 [7]|                                |
|MLDoc  | -----         | 95.25                          | 95.70 [2]| 88.75 [4]                      |
|DepPar | -----         | -----                          | 92.3/86.5 [2]| 
|MLQA   | -----         | -----                          | 64.3/46.6 [9]| 68.0/49.8 [10]
|XQuAD  | -----         | -----                          | 74.30 [11] |

## References

* [1] [Original Multilingual BERT](https://github.com/google-research/bert/blob/master/multilingual.md)
* [2] [Multilingual BERT on "Beto, Bentz, Becas: The Surprising Cross-Lingual Effectiveness of BERT"](https://arxiv.org/pdf/1904.09077.pdf)
* [3] [Multilingual BERT on "How Multilingual is Multilingual BERT?"](https://arxiv.org/pdf/1906.01502.pdf)
* [4] [LASER](https://arxiv.org/abs/1812.10464)
* [5] [XLM (MLM+TLM)](https://arxiv.org/pdf/1901.07291.pdf)
* [6] [UDPipe on "75 Languages, 1 Model: Parsing Universal Dependencies Universally"](https://arxiv.org/pdf/1904.02099.pdf)
* [7] [Multilingual BERT on "Sequence Tagging with Contextual and Non-Contextual Subword Representations: A Multilingual Evaluation"](https://arxiv.org/pdf/1906.01569.pdf)
* [8] [Multilingual BERT on "PAWS-X: A Cross-lingual Adversarial Dataset for Paraphrase Identification"](https://arxiv.org/abs/1908.11828)
* [9] [Multilingual BERT on "MLQA: Evaluating Cross-lingual Extractive Question Answering"](https://arxiv.org/abs/1910.07475)
* [10] [XLM on "MLQA: Evaluating Cross-lingual Extractive Question Answering"](https://arxiv.org/abs/1910.07475)
* [11] [JointMulti Multilingual BERT on "On the Cross-lingual Transferability of Monolingual Representations"](https://arxiv.org/abs/1910.11856)

## Summary

## XNLI

### Reported:

#### 73.15 [LASER](https://arxiv.org/abs/1812.10464)
#### 77.8 [Original Multilingual BERT repository](https://github.com/google-research/bert/blob/master/multilingual.md)
#### 78.5 [Multilingual BERT on "Beto, Bentz, Becas: The Surprising Cross-Lingual Effectiveness of BERT"](https://arxiv.org/pdf/1904.09077.pdf)
#### 80.8 [XLM (MLM+TLM)](https://arxiv.org/pdf/1901.07291.pdf)

### Ours

Best: 80.15

Detailed: experiments_XNLI.txt

## POS

### Reported

#### 96.71 [Multilingual BERT on "How Multilingual is Multilingual BERT?"](https://arxiv.org/pdf/1906.01502.pdf)
#### 97.1 [Multilingual BERT on "Beto, Bentz, Becas: The Surprising Cross-Lingual Effectiveness of BERT"](https://arxiv.org/pdf/1904.09077.pdf)
#### 98.91 [UDPipe on "75 Languages, 1 Model: Parsing Universal Dependencies Universally"](https://arxiv.org/pdf/1904.02099.pdf)

### Ours

Best: 98.44

Detailed: experiments_POS.txt

## NER CoNLL2002

### Reported

#### 87.18 [Multilingual BERT on "How Multilingual is Multilingual BERT?"](https://arxiv.org/pdf/1906.01502.pdf)
#### 87.38 [Multilingual BERT on "Beto, Bentz, Becas: The Surprising Cross-Lingual Effectiveness of BERT"](https://arxiv.org/pdf/1904.09077.pdf)

### Ours

Best: 81.7

Detailed: experiments_NER.txt

## NER WikiAnn

### Reported

#### 92.5 [Multilingual BERT on "Sequence Tagging with Contextual and Non-Contextual Subword Representations: A Multilingual Evaluation"](https://arxiv.org/pdf/1906.01569.pdf)

### Ours

## MLDoc

### Reported

#### 88.75 [LASER](https://arxiv.org/abs/1812.10464)
#### 95.7 [Multilingual BERT on "Beto, Bentz, Becas: The Surprising Cross-Lingual Effectiveness of BERT"](https://arxiv.org/pdf/1904.09077.pdf)

### Ours

## Dependency Parsing

### Reported

#### 92.3/86.5 [Multilingual BERT on "Beto, Bentz, Becas: The Surprising Cross-Lingual Effectiveness of BERT"](https://arxiv.org/pdf/1904.09077.pdf)

### Ours

## PAWS-X

### Reported

#### 89 and 90.7 [Multilingual BERT on "PAWS-X: A Cross-lingual Adversarial Dataset for Paraphrase Identification"](https://arxiv.org/abs/1908.11828)

### Ours

Best: 89.55

Detailed: experiments_PAWSX.txt

## MLQA

### Reported

#### 64.3 / 46.6 [Multilingual BERT on "MLQA: Evaluating Cross-lingual Extractive Question Answering"](https://arxiv.org/abs/1910.07475)
#### 68.0 / 49.8 [XLM on "MLQA: Evaluating Cross-lingual Extractive Question Answering"](https://arxiv.org/abs/1910.07475)


## XQuAD

### Reported

#### 74.3 [JointMulti Multilingual BERT on "On the Cross-lingual Transferability of Monolingual Representations"](https://arxiv.org/abs/1910.11856)

### Ours
