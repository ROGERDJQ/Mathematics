# 随机变量
- 随机变量为样本点的函数，我们定义大写字母为随机变量(书中为希腊字母)，以w表示样本点，则有如D(w)=k，表示随机变量取k时所对应的样本点集合，因而属于单值映射。
- 分布函数，F(x) = P{D(w) < x}，可写作随机变量服从分布D(w) ~ F(x)。
## 性质
- 单增，有上下限，左连续

# 连续型随机变量
- 易知，由分布函数定义可得，连续型随机变量的分布函数为累积量，且连续，则p可称为密度函数，反映了随机变量取X附近时临近值的概率大小（delta x，见积分）
- 正态分布
    - 若有密度函数有如【xx】,以及标准正态分布，其中标准正态分布早x=0处取得最值，关于x=0对称；而sigma表现分布的集中程度，sigma越小，越集中在x=a附近，
- 埃尔兰分布
    - 核心是**从二项分布到泊松分布**，很明了

- 多维随机变量【更重要】
    - 对同一样本点有不同随机变量的映射，那么对于这些随机变量而言，则组合构成一个n维的随机**向量**，亦是n维随机变量。
- 连续型 多元随机变量
    - 均匀分布
    - n元正态分布 【待补充】
- 边际分布
    - 本质上起名应当是来源于列联表。
    - 边际分布不能推出联合分布，也就是说多维(元)随机变量的分布性质是不能由个别分量的分布性质推出。
    - 二元正态分布的边际分布仍为正态分布 【推导较为模糊】 
- 条件分布
    - 引出随机变量独立
- 随机变量的函数，某些情况下可以与期望与方差的运算类似
    - 通过分布函数推导概率密度
    - 意外涉及到卷积与反函数，使得概率论与微积分联系在了一起【还要详细学习】
    - 基本思路有 已知x的概率密度函数以及分布函数，求与X有关的Y 的分布函数，将Y 的分布转化为X的分布即可，因此要求有对应的反函数
    - 均匀分布可以用来生成其他分布
- 多元正态分布正交变换后可以化为多个独立正态分布之积。