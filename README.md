# bigdata2
任务1：编写MapReduce程序，统计数据集中违约和⾮违约的数量，按照标签TARGET进⾏输出，即1代表有违约的情况出现，0代表其他情况。
该任务的思路与mapreduce的Wordcount例子相似，由于读入的文件变为了csv，这里先把第一行过滤后按照列编号得到TARGET的值。
![image](https://github.com/Aristellaaa/bigdata2/assets/127272945/d7ae1202-d1dc-40b7-b94e-f6f6ea7064c6)
reduce和其余部分与Wordcount均相同，不再详述。
输出结果见output：
![image](https://github.com/Aristellaaa/bigdata2/assets/127272945/a254cd8e-2dac-48f7-a432-f85279e73c9b)

任务2：编写MapReduce程序，统计⼀周当中每天申请贷款的交易数WEEKDAY_APPR_PROCESS_START，并按照交易数从⼤到⼩进⾏排序。
总体思路与任务1相似，不同的点在于需要对输出结果根据value进行排序，这里使用了java的TreeMap类来对键值对进行排序。
![image](https://github.com/Aristellaaa/bigdata2/assets/127272945/ad3a4031-3d73-475a-9d90-89be60006e5d)
如图，在排序完成后再将结果输出。

