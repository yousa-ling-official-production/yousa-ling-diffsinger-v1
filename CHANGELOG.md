# 更新日志


## V1.5

2024/10/20
- 修复了一些训练时的BUG，可能提高了多语言的表现
- 修复了部分音素缺失的问题（临时措施）


## V1.43e

2024/09/08
- 修复了在非常极端情况下输出依然超越上下界的问题
- 修复了pitch模型的组件缺失问题


## V1.43d

2024/09/05
- 修复了超音域音符导致程序崩溃的bug
- 清理了无用的词典文件


## V1.43c

2024/08/29
- 同步到multi-dict分支
- 支持英文（EN）
- 修复了日语孤立元音发音后延的问题
- 支持faster nsf，略微加快了渲染速度


## V1.43bJPCN_TEST

2024/06/14
- 修复了词典中部分辅音被标注为元音的bug
- 支持lynxnet_large


## V1.43JPCN_TEST

2024/06/05
- 支持日语
- voicing参数限时回归


## V1.42

2024/05/15
- 从该版本开始，将会分别发布使用LynxNet与WaveNet的版本
- 最新的LynxNet在保留过往优势（更快的渲染速度、更广的音域、更精准的咬字）的前提下修复了过往音色还原不准确的问题
- 此外依然提供OpenVPI/DiffSinger主线分支的WaveNet版本
- 采用了[transformer-parallel][8]提高8%的渲染速度
- 翻新了autopitch，现在不同声线渲染的pitch会有不同声线带来的风格差异


## V1.41ReFlow

2024/04/18
- ReFlow正式发布


## V1.41_RF_wavenet0416

2024/04/16
- ReFlow测试，wavenet对照


## V1.41_RF_lynxnet0414

2024/04/14
- ReFlow测试
- 修改了数据增强参数，增强了音域表现


## V1.41_RF_lynxnet0412

2024/04/12
- ReFlow测试
- 添加了Classic声线，更类似yousa早期的声线


## V1.41_RF_lynxnet

2024/04/05
- ReFlow测试，新的模型类别
- 声学模型网络结构由WaveNet修改为了[LynxNet][7]


## V1.41

2024/04/01
- 取消了对voicing参数的支持


## V1.4CE with AL

2024/03/06
- "CE" = Compact Edition
- 根据用户建议，恢复了Joyful声线
- 声学模型网络结构由WaveNet修改为了[LynxNet][7]，提高了音域边缘的生成质量，些微提升咬字精准度，大幅加快推理速度


## V1.4 with AL

2024/03/01
- 重新训练了权重，解决了V1.4dev2在高加速倍率下音质表现不佳的问题，但依然建议在低加速倍率下（如x10）导出作品
- 唱法模型上加入了主动学习（Active Learning）进行增强，添加了社区中的优秀调教作品作为参考，感谢社区用户的贡献
- 使用了最新版本的社区声码器并进行了微调，可以得到更好的音质表现
- 添加了新的参数voicing，同时删除了energy的支持，避免和tension参数的冲突
- 调整了默认的音色选择，现在默认音色为'Bright'


## V1.4dev2

2024/02/02
- 解决了expr参数莫名其妙没导出的问题
- 用onnxslim重新导出了声码器，我也不知道有没有变快
- 不改版本号了反正没什么区别


## V1.4dev

2024/02/01
- 重新训练
- 添加tension参数，注意这并不是目前本引擎正式版本支持的功能，需要配合[该仓库release的openutau][6]
- 改善了响度表现
- 改善了部分音区的音色表现
- 删除了Joyful、Soft两个声线


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
 [6]: https://github.com/haru0l/OpenUtau/releases
 [7]: https://github.com/CNChTu/DiffSinger
 [8]: https://github.com/openvpi/DiffSinger/pull/191