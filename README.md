（1）风险事件分类的训练集规模是10000+，包含10个一级标签和35个二级标签；大规模无标注的文本规模是亿级。数据性质均为新闻资讯数据，经过加密处理；
（2）使用的预训练模型：nezha，roberta, macbert;
（3）预训练策略：使用albert的ngram mask任务来替代mlm任务，新增一个structbert里提到的
word struct prediction 任务，随机打乱连续的三个词，让模型来还原这三个词;
（4）微调使用到的trick：PGD对抗训练；UDA中的TSA；自定义的模型架构；EMA；lookahead；



决赛成绩：A榜第4名；B榜第7名
