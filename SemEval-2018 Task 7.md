# SemEval-2018 Task 7
## 关系提取与关系分类被区分对待
- 关系提取:给定文本所有实体，提取有关系的实体对并对关系分类
- 关系分类:给定文本的实体对，对实体关系分类
## Evaluation metrics
### subtask 1.1 Relation classification on clean data
### subtask 1.2 Relation classification on noisy data
- for every distinct class: precision, recall and F1-measure (β=1)
- global evaluation, for the set of classes:
- macro-average of the F1-measures of every distinct class
- micro-average of the F1-measures of every distinct class
### subtask 2 Relation extraction and classification on clean data
#### extraction task
- precision:percentage of pairs of entities that were correctly connected (directionality and relation labels are ignored)
- recall: percentage of pairs of entities connected in the gold standard that were found (directionality and relation labels are ignored)
- F1-score (β=1): harmonic mean of precision and recall.
#### classification tasks
- Precision: percentage of relation instances that were correctly connected, with a correct directionality and a correct label assignment. Erroneously extracted instances which are not in the gold standard, instances labeled with ANY,  and instances with a wrong directionality are considered as wrong predictions.
- Recall: percentage of relation instances belonging to a specific relation in the gold standard that were found, with a correct directionality and correct label assignment.
- F-measure (β=1): harmonic mean of previous precision and recall
