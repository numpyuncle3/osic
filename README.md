竞赛地址：https://www.kaggle.com/c/osic-pulmonary-fibrosis-progression
建模思路：1.使用常规boost模型，依据提供的表格信息进行预测；2.使用深度神经网络模型，根据提供的病人CT图像预测病人肺活量的衰退系数，再乘以时间作为结果。
深度神经网络的思路基于病人的肺活量是线性变化的，但是经过分析，病人的肺活量与线性模型的残差很大，放弃了深度神经网络的思路。最终结果是lightgbm,xgboost,catboost的线性融合结果。
