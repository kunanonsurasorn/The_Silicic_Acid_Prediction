# โปรเจคการทำนายปริมาณกรดซิริซิคในทะเลของประเทศเกาหลีใต้

## 1. วัตถุประสงค์ 

     1.1 เพื่อทำนายปริมาณกรดซิริซิคในน้ำทะเล
 
     1.2 เพื่อหาโมเดลที่เหมาะสมทำนายปริมาณกรดซิริซิค

## 2. ชุดข้อมูล

     2.1 ชุดข้อมูลที่ใช้มาจากหน่วยงานสถิติของประเทศเกาหลีใต้ (Korean Statistical Information Service) 
 
     2.2 เว็บไซต์ของหน่วยงานสถิติเกาหลีใต้ : https://kosis.kr/eng/

## 3. ภาษาที่ใช้ในการเขียนโปรแกรม

     ภาษาที่ใช้ในการเขียนโปรแกรมคือ Python

## 4. Python Libraries 

     4.1 Numpy

     4.2 Pandas
 
     4.2 Matplotlib
 
     4.3 Seaborn
 
     4.4 Sklearn

     4.5 XGBoost

     4.6 Statsmodels

## 5. Data Visualization Tools

     5.1 Box Plot

![Boxplot_Silicic](https://raw.githubusercontent.com/kunanonsurasorn/The_Silicic_Acid_Prediction/refs/heads/main/Boxplot_Silicic.png)

     5.2 Histogram

![Histogram_Silicic](https://raw.githubusercontent.com/kunanonsurasorn/The_Silicic_Acid_Prediction/refs/heads/main/Histogram_Silicic.png)

     5.3 Correlation Table

![Correlationtable_Silicic](https://raw.githubusercontent.com/kunanonsurasorn/The_Silicic_Acid_Prediction/refs/heads/main/Correlationtable_Silicic.png)

     5.4 Scatter Plot

![Scatterplot_Silicic](https://raw.githubusercontent.com/kunanonsurasorn/The_Silicic_Acid_Prediction/refs/heads/main/Scatterplot_Silicic.png)
     
## 6. Models

     6.1 DecisionTreeRegressor()

     6.2 GradientBoostingRegressor()

     6.3 RandomForestRegressor()

     6.4 XGBRegressor()

## 7. Hyperparamter Tuning Methods

     7.1 GridSearchCV

     7.2 RandomizedSearchCV

## 8. ผลลัพธ์

     8.1 Coefficient of Determination between Normal Models (NS), GridsearchCV Models (GM) and RandomizedSearchCV Models (RM)
     
          8.1.1 DecisionTreeRegressor() Model
          
               - Coefficient of Determination(NS): 0.4925 
               
               - Coefficient of Determination(GM): 0.5176 
               
               - Coefficient of Determination(RM): 0.5306
               
          8.1.2 GradientBoostingRegressor() Model
          
               - Coefficient of Determination(NS): 0.7437 
               
               - Coefficient of Determination(GM): 0.7358 
               
               - Coefficient of Determination(RM): 0.7358
               
          8.1.3 RandomForestRegressor() Model
          
               - Coefficient of Determination(NS): 0.7704 
               
               - Coefficient of Determination(GM): 0.77 
               
               - Coefficient of Determination(RM): 0.7652
               
          8.1.4 XGBRegressor() Model
          
               - Coefficient of Determination(NS): 0.7305 
               
               - Coefficient of Determination(GM): 0.7305 
               
               - Coefficient of Determination(RM): 0.7305
               
     8.2 Coefficient of Determination between GridsearchCV Models (IGM) and RandomizedSearchCV Models (IRM)
     
          8.2.1 DecisionTreeRegressor() Model
          
               - Coefficient of Determination(IGM): 0.248 
               
               - Coefficient of Determination(IRM): 0.2765
               
          8.2.2 GradientBoostingRegressor() Model
          
               - Coefficient of Determination(IGM): 0.4298 
               
               - Coefficient of Determination(IRM): 0.4298
               
          8.2.3 RandomForestRegressor() Model
          
               - Coefficient of Determination(IGM): 0.4684 
               
               - Coefficient of Determination(IRM): 0.4794
               
          8.2.4 XGBRegressor() Model
          
               - Coefficient of Determination(IGM): 0.4683 
               
               - Coefficient of Determination(IRM): 0.4683

     8.3 ในโมเดลทั้งหมด 24 โมเดลให้เลือกใช้โมเดล RandomForestRegressor() แบบ Normal Models เพราะให้ค่า Coefficient of Determination 0.7704 เป็นค่าที่สูงที่สุดในกลุ่มโมเดลทั้งหมด

