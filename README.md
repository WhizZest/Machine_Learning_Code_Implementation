# 机器学习 公式推导与代码实现
李航老师的《统计学习方法》和周志华老师的西瓜书《机器学习》一直国内机器学习领域的经典教材。本书在这两本书理论框架的基础上，补充了必要的代码实现思路和逻辑过程。

本书在对全部机器学习算法进行分类梳理的基础之上，分别对监督学习单模型、监督学习集成模型、无监督学习模型、概率模型4个大类26个经典算法进行了相对完整的公式推导和必要的代码实现，旨在帮助机器学习入门读者完整地掌握算法细节、实现方法以及内在逻辑。本书可作为《统计学习方法》和西瓜书《机器学习》的补充材料。

---
### 使用说明
本仓库为《机器学习 公式推导与代码实现》一书配套代码库，相较于书中代码而言，仓库代码随时保持更新和迭代。目前仓库只开源了全书的代码，全书内容后续也会在仓库中开源。本仓库已经根据书中章节将代码分目录整理好，读者可直接点击相关章节使用该章节代码。

---
### 纸质版
<img 
src="https://github.com/luwill/louwill-python-learning/raw/master/cover.jpg"
width = "280" height = "350">
<br>
<div style="color: #999;
font-size:11px;
padding: 2px;"></div>

购买链接：[京东](https://item.jd.com/13581834.html) | [当当](http://product.dangdang.com/29354670.html)

---
### 配套PPT
为方便大家更好的使用本书，本书也配套了随书的PPT，购买过纸质书的读者可以在机器学习实验室公众号联系读者获取。

---
### 全书勘误表
#### 第一版第一次印刷勘误
|  序号   | 所在页码  | 具体问题 | 勘误类型 | 修改 |
|  ----  | ----  | ----  | ----  | ----  |
| 1  | 彩插第1页 | 图3-6逻辑回归描述与正文不统一 | 文字或格式错误 | 逻辑回归应改为对数几率回归 |
| 2  | 11 | 代码第4行 | 技术错误 | #矩阵点乘 应改为 #矩阵乘法 |
| 3  | 32 | 式3-9 | 技术错误 | 中间+号应为x号 |
| 4  | 37 | 代码3-5倒数第4和第6行  | 文字或格式错误 | lables 应改为labels |
| 5  | 43 | 图4-1缺少横纵坐标名称 | 建议 | 应补充横坐标为w1，纵坐标为w2 |
| 6  | 44 | 图4-2缺少横纵坐标名称 | 建议 | 应补充横坐标为x，纵坐标为y |
| 7  | 47 | 代码4-3倒数第19行参数少了个0.1 | 技术错误 | 应补全为l1_loss(x,y,w,b,0.1) |
| 8  | 50 | 图4-4缺少横纵坐标名称 | 文字或格式错误 | 应补充横坐标为w1，纵坐标为w2 |
| 9  | 52 | 代码4-8第7行参数少了个0.1 | 技术错误 | 应补全为l2_loss(x,y,w,b,0.1) |
| 10 | 68 | 代码6-6倒数第一行多一个右括号 | 文字或格式错误 | 去掉该括号 |
| 11 | 70 | 代码6-8第9和11行没有对齐 | 文字或格式错误  | 应与其他行对齐 |
| 12 | 71 | 该页Kneighbors中的n应大写 | 文字或格式错误 | 应改为KNeighbors |
| 13 | 77 | 表7-3数字统计错误 | 技术错误 | 应改为正确的统计数值：将“晴”和“雨”两行数值互换，相应的表格后第一个式子E(3,2)改为E(2,3)，E(2,3)改为E(3,2) |
| 14 | 79 | 倒数第四行名词错误 | 技术错误 | 应将信息增益比改为基尼指数 |
| 15 | 90 | 代码7-10中部分变量命名不统一 | 技术错误 | 应统一best_subsets、left_branch、feature_ix、leaf_value_calc等变量 |
| 16 | 92 | 代码7-11倒数第3行变量有误 | 技术错误 | 应将impurity_calculation改为gini_impurity_calc，\_leaf_value_calculation改为leaf_value_calc |
| 17 | 111 | 代码8-12倒数第9行  | 技术错误  | 多了一个parameter参数，应去掉  |
| 18 | 119 | 第一段第一行L(x,α,β)有误 | 技术错误  | 应改为L(w,b,α) |
| 19 | 121 | 式9-35缺少q矩阵部分  | 技术错误  | 应补充q矩阵 |
| 20 | 167 | 图12-1倒数第2行最优点式子有误 | 技术错误 | 应改为式12-18 |
| 21 | 211 | 第二段n个样本描述有误  | 技术错误 | 应改为m个样本，相应的式17-8求和上标改为n|
| 22 | 216 | 代码17-7第12行函数参数写反 | 技术错误  | 应对调修改 |
| 23 | 244 | 代码21-5倒数第6行可以与上一行进行合并 | 建议 | 应合并为一行 |

**注意：以上勘误在2022.2第二次印刷版本中均已更正！**

#### 第一版第二次印刷需勘误之处
|  序号   | 所在页码  | 具体问题 | 勘误类型 | 修改 |
|  ----  | ----  | ----  | ----  | ----  |
| 1 | 21 | 式2-8和2-9后两项w漏掉转置T | 技术错误 | 应补上转置T|
| 2 | 21 | 式2-6少一列 | 技术错误 | 应在矩阵最后补充1向量列，相应的描述应改为m*（d+1）维 |
| 3 | 29 | 代码2-8输出第二行 | 技术错误 | 应保留两位小数：0.54 |
| 4 | 33 | 第3段第3行“则式（3-13）可表示为”应补充描述 | 建议 | 应补充描述为“则式（3-13）似然项可表示为” |
| 5 | 40 | 代码3-9第一行和最后一行函数名有误 | 技术错误 | 应统一为plot_decision_boundary |
| 6 | 99 | 第2段第2行漏掉>0且式8-3w\*x+b缺少绝对值符号 | 技术错误 | 应改为“都有-y_i(wx_i+b)>0成立”并补充式8-3绝对值符号 |
| 7 | 145 | 倒数第2段中的t | 技术错误 | t应改为T |
| 8 | 155 | 最后一段式（11-10） | 文字或格式错误 | （11-10）应改为（11-9）|
| 9 | 169-170 | 代码12-1倒数第2、3行impurity_calculation、\_leaf_value_calculation与决策树一章变量不统一 | 文字或格式错误 | 应统一为gini_impurity_calc、leaf_value_calc |
| 10 | 225 | 式（19-11）多了一个VTV | 技术错误 | 去掉末尾的VTV即可 |
| 11 | 241 | 代码21-1倒数第2行和第12行class_condition_prob变量名未统一 | 技术错误 | 统一为prior_condition_prob |
| 12 | 242 | 代码21-2倒数第5行未缩进，以及prior命名未统一 | 技术错误 | 应缩进该行，并将prior命名统一为class_prior |
| 13 | 248 | 代码21-8倒数第4和第6行student_model和student_infer命名未统一 | 技术错误 | 应统一为letter_model和letter_infer |

**注意：以上勘误在2022.3第三次印刷版本中均已更正！**

#### 第一版第三次印刷需勘误之处
|  序号   | 所在页码  | 具体问题 | 勘误类型 | 修改 |
|  ----  | ----  | ----  | ----  | ----  |
| 1 | 86 | 倒数第三行均方损失 | 技术错误 | 应改为平方损失 |
| 2 | 126 | 第二段式（9-40） | 技术错误 | 应改为式（9-39） |
| 3 | 225 | 式19-8与式19-9 A与AT写反 | 技术错误 | 式19-8应改为AAT，式19-9应改为ATA，对应公式下的变量和描述也随公式进行修正 | 
| 4 | 265 | 式23-22、23-24、式23-25局部有误 | 技术错误 | 式23-22、23-24条件概率\|应在Ot后，式23-25倒数第二个式最后一个\|应为逗号 |

---
### LICENSE
本项目采用[知识共享署名-非商业性使用-相同方式共享 4.0 国际许可协议](https://creativecommons.org/licenses/by-nc-sa/4.0/)进行许可。
