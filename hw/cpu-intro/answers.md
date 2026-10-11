# CPU Intro Homework

## Q1
- Prediction: 10
- Reasoning: 每条指令执行需要1个周期，一共10条指令，总周期数为10。
- Verified result:10
- Analysis:No hazards in this instruction sequence. There are no stalls, so the simulated cycle count matches our prediction.

## Q2
- Prediction: 14
- Reasoning: 有4条stall阻塞指令，10条基础指令周期，10+4=14。
- Verified result:14
- Analysis:Data hazards exist between instructions and create stalls. The final cycle number is consistent with our estimate.

## Q3
- Prediction: 11
- Reasoning: 存在1次数据依赖产生阻塞，基础10周期，加上1个stall，合计11。
- Verified result:11
- Analysis:Minor data stalls appear. The simulation result agrees with the predicted value.

## Q4
- Prediction: 16
- Reasoning: 存在6次数据依赖阻塞，基础10周期，加上6，总周期数为16。
- Verified result:16
- Analysis:Multiple instructions have data dependencies, which cause several stalls and increase total cycles

## Q5
- Prediction: 13
- Reasoning: 存在3次冒险阻塞（数据+分支控制冒险），基础10周期，加上3，总周期数为13。
- Verified result:13
- Analysis: Branch instruction introduces control hazard, adding extra cycles. Simulation matches prediction.

## Q6
- Prediction: 12
- Reasoning: 存在2次数据依赖阻塞，基础10周期，加上2，总周期数为12。
- Verified result:12
- Analysis:Only a small number of data stalls. The real cycle count is the same as our prediction.

## Q7
- Prediction: 18
- Reasoning: 存在8次连续数据依赖阻塞，基础10周期，加上8，总周期数为18。
- Verified result:18
- Analysis:Consecutive data hazards create many stalls, leading to the longest cycle count among these questions.

## Q8
### Q8-S1
- Prediction: 14
- Reasoning: 分支预测失败，产生4次控制阻塞，基础指令加上4个stall，合计14。
- Verified result:14
- Analysis:Branch prediction fails, resulting in control stalls and extra cycles.
### Q8-S2
- Prediction: 12
- Reasoning: 部分分支预测成功，stall减少到2，总周期12。
- Verified result:12
- Analysis:Partial successful branch prediction reduces the number of stalls.
### Q8-S3
- Prediction: 10
- Reasoning: 所有分支全部预测命中，无阻塞，总周期10。
- Verified result:10
- Analysis:All branches are predicted correctly. No control stalls occur.
