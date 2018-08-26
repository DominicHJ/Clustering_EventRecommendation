## Clustering_EventRecommendations  

### 简介   
在kaggle竞赛Event Recommendation Engine Challenge数据集上，根据活动的关键词（count_1, count_2, ..., count_100，count_other属性）对样本进行聚类，由于样本数目较多（用户3w+），本项目使用MiniBatchKMeans。   

### 数据集   
数据来源于Kaggle竞赛：Event Recommendation Engine Challenge，根据events they’ve responded to in the past user demographic information what events they’ve seen and clicked on in our app 用户对某个事件是否感兴趣      

样本特征包括： 
- user_id    
- locale：地区，语言    
- birthyear：出身年    
- gender：性别    
- joinedAt：用户加入APP的时间，ISO-8601 UTC time    
- location：地点    
- timezone：时区       
- count_N：活动描述出现第N个词的次数     
- count_other：除了最常用的100个词之外的其余词出现的次数     
注：后101列为词频：count_1, count_2, ..., count_100，count_other     
![](dataset _overview.png 'dataset _overview')      

竞赛官网：https://www.kaggle.com/c/event-recommendation-engine-challenge/data   
 
