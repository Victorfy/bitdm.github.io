该文档包含两种代表算法，和其中一个例子

## 聚类算法：k-means算法学习

算法步骤：
- 从N个文档随机选取K个文档作为质心
- 对剩余的每个文档测量其到每个质心的距离，并把它归到最近的质心的类
- 重新计算已经得到的各个类的质心
- 迭代2～3步直至新的质心与原质心相等或小于指定阈值，算法结束

matlab中有kmeans函数

##两种概念的理解和区分：classification,cluster
* 聚类(clustering)：处理过程中不使用对象的类别信息，只根据各特征值将对象进行“物以类聚”；
* 分类(classification)：处理过程中时时受到对象类别信息的影响（监督），算法在选择特征、选择阈值等步骤时都要使得具有相同类别标签的对象在一起，而具有不同类别的对象不在一起。
* 可以说分类是已知对象预先已经被分类，算法的目的是要把未知对象赋类别标签；而聚类则不管已知未知，通通当做未知类别标签，把已知未知放在一起“物以类聚”。
http://www.cnblogs.com/bangemantou/archive/2013/01/07/2850155.html

不知道这个理解是否正确

例子
http://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer-wisconsin/
http://www.cnblogs.com/asxinyu/p/3289682.html

## 分类算法：k-nearest neighbor(knn)
