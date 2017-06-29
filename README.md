# Tencent2017_Final_Rank28_code
2017第一届腾讯社交广告高校算法大赛Rank28_code
赛题详情：http://algo.tpai.qq.com/home/information/index.html

题目描述

计算广告是互联网最重要的商业模式之一，广告投放效果通常通过曝光、点击和转化各环节来衡量，大多数广告系统受广告效果数据回流的限制只能通过曝光或点击作为投放效果的衡量标准开展优化。腾讯社交广告(http://ads.tencent.com)
发挥特有的用户识别和转化跟踪数据能力，帮助广告主跟踪广告投放后的转化效果，基于广告转化数据训练转化率预估模型(pCVR，Predicted Conversion Rate)，在广告排序中引入pCVR因子优化广告投放效果，提升ROI。

本题目以移动App广告为研究对象，预测App广告点击后被激活的概率：pCVR=P(conversion=1 | Ad,User,Context)，即给定广告、用户和上下文情况下广告被点击后发生激活的概率。

代码描述




    按照代码标号顺序逐个生成特征csv文件，代码内有相应特征说明。生成特征之后运行lgb和xgb文件模型代码分别得到2个模型的预测结果。
    
    ##代码运行之前下载决赛数据集（http://spabigdata-1253211098.cosgz.myqcloud.com/final.zip），解压至Tencent文件夹下。
    
    最终提交特征由基础特征，交叉特征，统计特征，转化率特征和trick特征组成，共计100维左右，建议运行在32G内存以上机器。
    
    模型方面用到xgboost,lightgbm,第一次参赛，经验不足，决赛前期因线上线下得分不一致，花费太多时间在数据集构建上，导致没有充分的时间筛选特征，
    没有stacking融合，模型参数也没有调到最优，遗憾未能进入前二十。
    
    最终提交结果得分：0.101972，由xgb,lgb预测结果平均得到。

