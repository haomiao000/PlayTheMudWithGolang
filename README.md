# Dormitory-Distribution-System
This project is an innovation and entrepreneurship project for college students of Harbin University of Science and Technology



## About Dormitory-Distribution-System

目前，我国高校宿舍分配主要依赖传统的人工方式，宿舍管理人员，如学生宿舍宿务辅导员，会主观评估学生的地域背景、学术成绩、性格特点、民族差异等因素，并采用地域搭配法、成绩搭配法、性格搭配法以及民族搭配法等方法来进行宿舍分配的决策。然而，这些传统的人工宿舍分配方法存在诸多问题，如效率低、效果差、主观性强、随机性大等，已无法满足当代大学生对个性化宿舍分配的需求。

所以我们的项目致力于开发一款自动化的宿舍分配模型，以提高分配效率和准确性，推进宿舍管理的科技化和智能化进程。该模型能够客观地考虑学生的特点和偏好，避免主观评估和随机分配所带来的不确定性和不适应。同时，宿舍分配模型可以不断学习和优化，根据实际效果和反馈进行调整，逐渐提升分配的准确性和满意度。



## Why Dormitory-Distribution-System

因为遗传算法具有普适性、灵活性和强大的可扩展性，同时具备高效获取最优解的潜力

我们将基于多种群遗传算法MPGA进行个性化寝室室友匹配，通过种群的迭代和优胜劣汰的过程，遗传算法能够逐步改进解的质量，使得适应度不断收敛于最优值。通过选择、交叉和变异等操作，优秀的个体特征可以得到保留和传递，从而使种群中的解越来越接近最优解。最终，遗传算法能够找到一个相对优秀的解，对于复杂的问题具有较好的解决能力。遗传算法相比与其他算法有以下优点：

（1）全局搜索能力：遗传算法以随机生成初始种群为基础，通过遗传操作和选择操作不断迭代优化，具有全局搜索的能力，可以在解决问题时找到全局最优解。

（2）适应性强：遗传算法对于问题空间中的非线性、多峰和多模态问题具有良好的适应性，可针对不同的宿舍分配需求进行优化。

（3）可扩展性好：遗传算法的模型结构相对简单，且可以通过调整遗传算子参数、增加或减少种群规模等方法进行优化，因此具有较好的可扩展性。

（4）非确定性优化：遗传算法是一种基于概率的优化方法，与其他传统的确定性优化方法相比，其能够在大规模问题中表现出更好的优化效果。

（5）并行计算：遗传算法的并行化实现比较容易，利用高性能计算资源进行并行化计算能够显著提高算法的效率和速度。



## Work flow

![](/images/workflow.png)

# vue

## 运行Vue

### step1：安装vue
```
npm install
```

### step2：终端输入运行vue文件

```
npm run serve
```

#### json-server的安装

```c
//安装json
npm install -g json-server
json-server db.json
```

解释：所有的网络请求的 json 统一放在了 db.json 里给前端网络请求提供数据

### python 运行：
python 文件夹下运行
`python Allocation.py --dbpath "数据库路径"`
`python3 Allocation.py --dbpath /Users/hao/Desktop/go/Dormitory-Distribution-System/gorm.db`

### drop
drop table user_questionnaire_data;
drop table user_base_infos;

### select
select * from user_questionnaire_data;
select * from user_base_infos;

PRAGMA table_info(user_base_infos);

python3 ./python/Allocation.py --dbpath gorm.db --image del.png --rounds=1000 --end_bound=100
python3 ./python/Allocation.py --dbpath gorm.db --image del.png --rounds=1000 --end_bound=100