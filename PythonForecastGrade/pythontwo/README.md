#   学生总成绩预测
使用python编程，KNN算法实现同学成绩预测，预测学生整学期平均成绩
预测对象：同学期末成绩。
测试数据集在附录中，包含：每学期学习所消耗的时间（小时），每周娱乐所消耗平均时间（小时），每天上课平均坐前排平均次数比值。
预测结果为期末成绩不及格，及格，优秀
#  KNN算法
# k-近邻算法
      k-近邻算法（kNN)，它的工作原理是：存在一个样本数据集合，也称作训练样本集，并且样本集中每个数据都存在标签，即我们知道样本集中每一数据与所属分类的对应关系。输入没有标签的新数据后，将新数据的每个特征与样本集中数据对应的特征进行比较，然后算法提取样本集中特征最相似数据（最近邻）的分类标签。一般来说，我们只选择样本数据集中前k个最相似的数据，这就是k-近邻算法中k的出处，通常k是不大于20的整数。最后，选择k个最相似数据中出现次数最多的分类，作为新数据的分类。
# k近邻算法优缺点
优点：精度高、对异常值不敏感、无数据输入假定。
缺点：计算复杂度高、空间复杂度高。 适用数据范围：数值型和标称型。

#  训练模型
# 1.显示数据集
先使用可视化技术将数据集显示出来
颜色	黑色（fail）	黄色（Marginal）	红色（excellent）
结果集	不及格	及格	优秀
所测图一为：每学期学习所消耗的时间与每周娱乐所消耗平均时间比值
横坐标：每学期学习所消耗的时间（小时）
纵坐标：每周娱乐所消耗平均时间（小时）
所测图二为：每学期学习所消耗的时间与每天上课平均坐前排平均次数比值
横坐标：每学期学习所消耗的时间（小时）
纵坐标：每天上课平均坐前排平均次数比值
所测图三为：每周娱乐所消耗平均时间与每天上课平均坐前排平均次数
横坐标：每周娱乐所消耗平均时间（小时）
纵坐标：每天上课平均坐前排平均次数比值
所测图四为：每次作业平均完成比例与每天上课平均坐前排平均次数
横坐标：每次作业平均完成比例
纵坐标：每天上课平均坐前排平均次数比值
![image](https://github.com/Concealed0/PythonForecastGrade/blob/master/PythonForecastGrade/pythontwo/image/viewdata.png)
通过对比发现,在数据集每学期学习时间长的，每周玩的时间短，上课平均坐前排的同学，每次作业平均完成高的最终成绩比较优秀。

# 2对数据集测试
![image](https://github.com/Concealed0/PythonForecastGrade/blob/master/PythonForecastGrade/pythontwo/image/console-1.png)
# 测试结果：
![image](https://github.com/Concealed0/PythonForecastGrade/blob/master/PythonForecastGrade/pythontwo/image/console-2.png)
通过使用归一化将数据集进行分类，选取60%数据进行测试模拟，最终测试集错误率降低为0.0000%
#  模型测试

# 测试数据
每学期学习所消耗的时间（小时）:986
每周娱乐所消耗平均时间（小时）:23.5323
每天上课平均坐前排平均次数比值:0.76452
每次作业平均完成情况比例:0.6753
# 测试结果
测试的Variable explorer

测试的console
![image](https://github.com/Concealed0/PythonForecastGrade/blob/master/PythonForecastGrade/pythontwo/image/console-3.png)



