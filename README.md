# 2017-Industrial-Bigdata
- 首届（2017）中国工业大数据创新大赛[2017_Industrial_Bigdata_Innovation_Competition](http://www.industrial-bigdata.com/index.jsp?_t=1507361284976)
- Time：2017.06-2017.10
- Competition Topic:(风机叶片结冰预测大赛)[http://www.industrial-bigdata.com/competition/competitionAction!showDetail.action?competition.competitionId=1]

### 1.Introduction
This repository shares the process of Machine Learning to **predict whether the leaves of wind turbines are frozen**.In the homepage of competition, it introduces the detail information of competiton.The data come from a system called "SCADA" that can manage, monitor and control the whole wind field.The SCADA can provide environment parameters, technique parameters, control parameters and other parameters about running wind turbines.The data contains **28 continuous numerical variables**, that includes many dimension，such as technique parameters, environment parameters and so on.The following section describes the procedure to figure out **a binary classification problem** in detail. The main procedure flow incorporate **data-preprocessing -> feature-engineering -> metrics-selection -> model-building -> model-selection -> parameters-tuning -> predict testset**.

### 2.Procedure Flow
2.1 Data-Preprocessing
 - Mark up corresponding labels according to failure information
 - Drop out no-label examples
 - Exploratory data analysis - univariate analysis -> histogram & boxplot
 
2.2 Feature-Engineering
 - Generate polynomial Feature
 - Feature selection method -> filter & embedded & wrapper
 
2.3 Metrics-Selection
 - Imbalance data - sample method(detail in .ipython)
 - ROC & ACU & F1_score & coustom_metrics
 
2.4 Model-Building
 - Logistic model
 - RandomForest model
 - Gradient boosting desicion tree
 - Xgboost

2.5 Model-Selection
 - compare metrics score
 - compare execution time

2.6 Parameters-Tuning
 - learning_rate
 - n_estimators
 - max_depth
 - min_child_weight
 - gamma
 - subsample
 - colsample_bytree
 - reg_alpha
 - reg_lambda
 - scale_pos_weight

2.7 Predict testset

### 3.Conclusion
It is excited that applying ML knowledge try to figure out a real problem. Through the whole procedure flow of data mining， the practice can really enhance your data analysis technology.My final ranking is **52 in 830 teams** that is **top 6%**. Althrough  I am unfortunately out of final competition and the ranking is not good enough, I will keep going along the data science path!
