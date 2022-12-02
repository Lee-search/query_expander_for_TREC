# TREC-2022 Clinical Trials Track
# This document summarizes the Query Expansion process of the TREC-2022 project.

* TREC-2022 프로젝트의 질의 확장(Query Expansion) 과정을 개별 정리한 문서입니다.

```
https://trec.nist.gov/
https://trec-cds.org/2022.html
```


## Getting Started

* 아래의 파이썬 라이브러리를 설치
```
!pip install elasticsearch_dsl
!pip install transformers==2.11.0

!pip install tensorflow
!pip install spacy
!pip install gensim
!python -m spacy download en
```

## Process in .ipynb

### 1. Import Datasets (Terms by Bio-Clinical BERT)
* BioBERT, ClinicalBERT 를 통해 추출된 Terms 목록을 업로드

### 2. Run Expanding Module
* QEModule 을 사용해 질의 확장 진행

### 3. Save expanded terms by CSV
* 확장된 질의를 .CSV 파일로 저장

## Query Expansion Techniques
* https://colab.research.google.com/github/fastforwardlabs/ff14_blog/blob/master/_notebooks/2020-07-22-Improving_the_Retriever_on_Natural_Questions.ipynb#scrollTo=1xwiI8KJ7D1V

