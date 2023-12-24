# Prediction_median_house_value_SPARK

**Описание** 

В проекте необходимо обучить модель линейной регрессии на данных о жилье в Калифорнии в 1990 году. 
В колонках датасета содержатся следующие данные:

- longitude — широта;
- latitude — долгота;
- housing_median_age — медианный возраст жителей жилого массива;
- total_rooms — общее количество комнат в домах жилого массива;
- total_bedrooms — общее количество спален в домах жилого массива;
- population — количество человек, которые проживают в жилом массиве;
- households — количество домовладений в жилом массиве;
- median_income — медианный доход жителей жилого массива;
- median_house_value — медианная стоимость дома в жилом массиве;
- ocean_proximity — близость к океану.

**Цель** 

На основе данных предсказать медианную стоимость дома в жилом массиве — median_house_value. 

**Задачи** 

1. Обучить модель и сделайть предсказания на тестовой выборке.
2. Для оценки качества модели использовать метрики RMSE, MAE и R2.


**План действий:**

1. Инициализировать локальную Spark-сессию.
2. Прочитать содержимое файла housing.csv.
3. Вывести типы данных колонок датасета, используя методы pySpark.
4. Выполнить предобработку данных. 
       * Исследовать данные на наличие пропусков и заполнить их, выбрав значения по своему усмотрению. 
       * Преобразовать колонку с категориальными значениями техникой One hot encoding.
5. Построить две модели линейной регрессии на разных наборах данных:
       * используя все данные из файла;
       * используя только числовые переменные, исключив категориальные.
6. Для построения модели использовать оценщик LinearRegression из библиотеки MLlib.
7. Сравнить результаты работы линейной регрессии на двух наборах данных по метрикам RMSE, MAE и R2.
8. Сделайтб выводы.


**Description**

In the project, it is necessary to train a linear regression model on housing data in California in 1990. The columns of the dataset contain the following data:

- longitude — latitude;
- latitude — longitude;
- housing_median_age — the median age of the residents of the housing complex;
- total_rooms — the total number of rooms in the houses of the housing complex;
- total_bedrooms — the total number of bedrooms in the houses of the housing complex;
- population — the number of people living in the housing complex;
- households — the number of households in the housing complex;
- median_income — the median income of the residents of the housing complex;
- median_house_value — the median house value in the housing complex;
- ocean_proximity — proximity to the ocean.

**Objective**

To predict the median house value in a housing complex — median_house_value, based on the data.

**Tasks**

1. Train the model and make predictions on the test sample.
2. Use RMSE, MAE, and R2 metrics to evaluate the quality of the model.

**Action Plan:**

1. Initialize a local Spark session.
2. Read the contents of the housing.csv file.
3. Output the data types of the dataset columns using pySpark methods.
4. Perform data preprocessing. * Investigate the data for missing values and fill them in as you see fit. * Convert the column with categorical values using One-hot encoding technique.
5. Build two linear regression models on different datasets: * using all the data from the file; * using only numerical variables, excluding categorical ones.
6. To build the model, use the LinearRegression estimator from the MLlib library.
7. Compare the results of linear regression on the two datasets using RMSE, MAE, and R2 metrics.
8. Draw conclusions.
