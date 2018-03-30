## 数据集
- 该论文用的数据集是SemEval-2010,一共8000个句子,包含10种关系(包含其他关系种类)
- 该数据集考虑了关系的方向性,例如因果关系的谁是因谁是果,所以一共18种关系
- 评估指标为accuracy over all examples and macro-averaged F-score over the 18 relation labels apart from Other
- To calculate the F-score, 18 individual F-scores -- one for each relation label -- are calculated in the standard way and the average of these scores is taken.
- The official evaluation measures are accuracy over all examples and macro-averaged F-score over the 18 relation labels apart from Other. To calculate the F-score, 18 individual F-scores -- one for each relation label -- are calculated in the standard way and the average of these scores is taken. For each relation Rel, each sentence labelled Rel in the gold standard will count as either a true positive or a false negative, depending on whether it was correctly labelled by the system; each sentence labelled with a different relation or with Other will count as a true negative or false positive.
## 交叉验证
## Attention
- attention的对象是一个句子的每一个词
