## 示例演练
  
  - 创建机器学习工作区（workspace），不做解释
  
  - 上传现有的数据（本地csv）
  
  - 创建实验（Experiments）
    1. 选择数据集
    2. 对数据集基本操作，例如 Select columns Dataset、Clean Miss Data、Split Data、Join Data
    3. 选择合适的算法：主要分为三大类：监督学习、非监督学习、强化学习。也有介于监督学习和半监督学习之间的半监督学习。
      - 监督学习即有特定的数据集，对预期的目标进行预测。
        - 例如：决策树（Decision Tree）、贝叶斯分类算法（Native Dayesion Classification）、最小二乘法（Ordinary Least Squares Resgression）、逻辑回归（Logistic Regression）、支持向量机（Support Vector Machine即SVM）、组合方法（Ensemble Methods）
      - 非监督学习即指目标没有提前指定，存在潜在关系的。
        - 例如：聚类算法（Clustering Algorithms）、主成分分析（Principal Component Analysis，PCA）、奇异值分解（Singular Value Decomposition）、独立成分分析（Independent Component Analysis）
    4. Train Model  
    5.Score Model
    6.Evaluate Model
  - [定型和评估实验](https://docs.microsoft.com/zh-cn/azure/machine-learning/machine-learning-walkthrough-4-train-and-evaluate-models)
  
  - 部署web服务
    * Experiments -> Run -> Set Up Web service -> Deployee -> Publish
  
  - 访问Web服务
    - 两种方式：请求响应服务RRS（Request Response Service）、批量执行服务BES（Batch Excute Service）
    - RRS：向服务器发送一行或多行/返回一个或多个数据集。（APIURL、APIKEY、JSONBODY）
    - BES：将数据的一行或多行存储在Azure Blob,发送Blob位置到服务/服务对Blob的行分析将结果存储在另一个Blob，返回该Blob URL。  （APIURL、APIKEY、JSONBODY、JOBID）
    - [官方说明](https://docs.microsoft.com/zh-cn/azure/machine-learning/machine-learning-consume-web-services)
  
  - [ML机器学习文档](https://docs.microsoft.com/zh-cn/azure/machine-learning)
