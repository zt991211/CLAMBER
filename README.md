# CLAMBER: A Benchmark of Identifying and Clarifying Ambiguous Information Needs in Large Language Models
> **Co-first author**: Tong Zhang (Sichuan University), Peixin Qin (Sichuan University)

This is the benchmark test dataset, called **CLAMBER**, which is used to evaluate LLMs using a well-organized taxonomy in terms of identifying and clarifying ambiguous information needs.
## Paper
[Click Me](https://arxiv.org/abs/2405.12063)

## Ambiguity Taxonomy in the era of LLM
![Taxonomy](./taxonomy.png)

## Dataset Information

| Name                  | Meaning                       | Values                                                                                                                                                              |
|-----------------------|-------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| question              | user query                    | string                                                                                                                                                              |
| context               | context of user query         | string                                                                                                                                                              |
| clarifying_question   | suggested clarifying question | string                                                                                                                                                              |
| require_clarification | If user query is ambiguous    | 0/1                                                                                                                                                                 |
| category              | ambiguity type                | {"FD": "Epistemic Misalignment",  "MC": "Aleatoric Output", "LA": "Linguistic Ambiguity"}                                                                           |
| subclass              | sub-type                      | {"whom":  "WHOM", "what": "WHAT", "when": "WHEN", "where": "WHERE", "NK":  "UNFAMILIAR", "ICL": "CONTRADICTION", "co-reference": "SEMANTIC", "polysemy": "LEXICAL"} |



# Reference
If you make advantage of the DREditor in your research, please cite the following in your manuscript:

```
@misc{zhang2024clamber,
      title={CLAMBER: A Benchmark of Identifying and Clarifying Ambiguous Information Needs in Large Language Models}, 
      author={Tong Zhang and Peixin Qin and Yang Deng and Chen Huang and Wenqiang Lei and Junhong Liu and Dingnan Jin and Hongru Liang and Tat-Seng Chua},
      year={2024},
      booktitle = {Proceedings of the 62nd Annual Meeting of the Association for Computational Linguistics (ACL)},
}
```
