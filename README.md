# predict_agegroup_card_user_python_ML
предсказание возростной группы по покупкам


### Final score: 0,6167 (place:12)
	Best Public score: 0,6167
	Best Private score: 0,0


## Описание подхода

Всего признаков чуть больше 200 признаков:
  * Кол-во и сумма покупок
  * Кол-во задействованых услуг каждого клиента
  * По каждому клиенту ('sum','mean','std','min','max')
  

Моделирование происходит функцией взятой из базовой модели
Для построения моделей используется GradientBoostingClassifier. Так же рассматривались xgboost,lightgbm и RandomForestClassifier.


## Описание файлов:

	/описание задачи/ - краткая информация о соревновании и входных данных
	/data_in/ - входные данные
	/data_out/ - результат предсказания
	/code/ - модели

	model_v3.ipynb - Модель, обработка данных и предсказание модели в одном файле. 
	Лучший результат на GradientBoostingClassifier() - Public = 0,6144
	
	model_v5.ipynb - Модель, обработка данных и предсказание модели в одном файле. 
	Лучший результат на LGB() - Public = 0,6167
	
	submission_052249.csv - результат предсказания GBC() Public = 0,6144, Private = 0,0
	
	submission_160044.csv - результат предсказания LGB() Public = 0,6167, Private = 0,0




## Ссылки

Cайт соревнования [Гадаем на картах](https://ods.ai/competitions/sberbank-sirius-lesson)
