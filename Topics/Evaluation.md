# Evaluation

### Hallucinations
Question: How to Evaluate Halluations and Factuality in Large Language Model? What are the limitions of Common Metrics?

Keywords: Hallucination, Factuality, FActScore, Truthful QA

#### Short Answer

Hallucination evaluation should break responses down into verifiable atomic claims, then determine whether each claim is supported by the provided evidence or authoritative sources. The evaluation should seperately measure factual precision, coverage, and the proportion of unverifiable claims.

TruthfulQA, FActScore, Natural Language Inference (NLI), and LLM-as-a-Judge each address only part of the problem. A single overall score cannot represent factual errors across all domains.

Main idea: Hallucination evaluation is not about whether an entire response should plausible. It is about decomposing the response into claims, matching them with evidence, and verifying each claim individually.

#### Detailed Anwser

Factuality can be divied into at least two main categories: 
    - Internal consistency: The response does not contradict the provided context. 
    - External consistency: The claims are consistent with reliable real-world sources.

Summarization, RAG, and open-domain question answering have different evidence boundaries and therefore required different evaluation designs. 

For long-forms answers, break the response into atomic facts.

A precision-like metric can be caluateda as:


At the same time, evaluation depends on retrieval recall, evidence quality, and the capabilities of the evaluation model.




### Golden Dataset
