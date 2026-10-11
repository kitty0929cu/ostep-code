# CPU Intro Homework

## Q1
- Prediction: 10
- Reasoning: 每条指令执行需要1个周期，一共10条指令，总周期数为10。
- Verified result:
- Analysis:

## Q2
- Prediction: 14
- Reasoning: 有4条stall阻塞指令，10条基础指令周期，10+4=14。
- Verified result:
- Analysis:

## Q3
- Prediction: 12
- Reasoning: 存在2次数据依赖产生阻塞，基础10周期，加上2个stall，合计12。
- Verified result:
- Analysis:

## Q4
- Prediction: 10
- Reasoning: 指令顺序被编译器重排，消除了数据依赖，没有stall，一共10周期。
- Verified result:
- Analysis:

## Q5
- Prediction: 11
- Reasoning: 分支预测错误，产生1个stall，基础10周期，总共11周期。
- Verified result:
- Analysis:

## Q6
- Prediction: 10
- Reasoning: 分支预测全部命中，没有停顿，10条指令，总周期10。
- Verified result:
- Analysis:

## Q7
- Prediction: 13
- Reasoning: 内存加载带来3次stall，基础10周期，合计13周期。
- Verified result:
- Analysis:

## Q8
### Q8-S1
- Prediction: 18
- Reasoning: 高延迟内存访问，多次阻塞，基础指令加上8个stall，合计18。
- Verified result:
- Analysis:
### Q8-S2
- Prediction: 14
- Reasoning: 缓存命中，减少部分内存stall，stall减少到4，总周期14。
- Verified result:
- Analysis:
### Q8-S3
- Prediction: 10
- Reasoning: 全部缓存命中，无内存停顿，没有stall，总周期10。
- Verified result:
- Analysis:
