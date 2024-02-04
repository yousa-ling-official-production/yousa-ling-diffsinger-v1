# 更新日志


## V1.3

2023/12/26
- 修复了虽然添加了多种音色的支持但没有支持一点的bug
- 整理了杂乱的文件结构

## V1.3a

2023/12/23
- 取消了对日语的支持
- 添加对多种音色的支持

## V1.2

2023/12/09
- 添加音高预测模型


## V1.2-b3

2023/12/08
- 添加更新日志
- 添加LISENCES
- 继续训练了欠拟合的模型
- 重新对[声码器(OpenVPI)][4]进行微调
- 对词典的日语部分修改


## V1.2-b2

2023/12/06
- 重新训练音素时长模型，支持日语
- 训练数据加入[CODEY_dataset][5]
- 对[声码器(fishaudio)][3]进行微调


## V1.2-b1

2023/12/05
- 重新训练声学模型、能量与气声模型
- 全面优化数据标注，大幅提升声库易用性及性能
- 支持日语


## V1.1

2023/11/26
- 重新训练
- 引擎升级到[DiffsingerV2(OpenVPI)][2]
- 数据重新处理
- 添加音素时长模型
- 添加能量与气声模型
- 添加对ENE、BREC、GEN、VEL参数的支持
- 替换背景透明的立绘([yousa-ling-official-production/yousa-ling-diffsinger-v1#2][1])


## V1.0

2023/04/04
- 加入数据增强，重新训练
- 初次发布版本


## V1.0-0224

2023/02/24
- 数据重筛选，重新训练


## V1.0-0219

2023/02/19
- 最初版本





 [1]: https://github.com/yousa-ling-official-production/yousa-ling-diffsinger-v1/pull/2
 [2]: https://github.com/openvpi/DiffSinger
 [3]: https://github.com/fishaudio/fish-diffusion/releases/tag/v2.0.0
 [4]: https://openvpi.github.io/vocoders/
 [5]: https://github.com/KakaruHayate/CODEY_Dataset