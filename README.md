# predict_agegroup_card_user_python_ML
предсказание возростной группы по покупкам


### Final score: 0,0 (place:None)
	Best Public score: 0,06144
	Best Private score: 0,0


## Описание подхода

Всего признаков чуть больше 200 признаков:
  * Кол-во и сумма покупок
  * Кол-во задействованых услуг каждого клиента
  * По каждому клиенту ('sum','mean','std','min','max')
  

Моделирование происходит функцией взятой из базовой модели
Для построения моделей используется GradientBoostingClassifier. Так же рассматривались xgboost,lightgbm и RandomForestClassifier.


## Описание файлов:

	информация.docx - краткая информация о соревновании
	данные.docx - краткая информация о входных данных

	model_v3.ipynb - Модель, обработка данных и предсказание модели в одном файле. 
	Лучший результат на GradientBoostingClassifier() - Public = 0,6144
	
	submission_052249.csv - результат предсказания Public = 0,6144, Private = 0,0




## Ссылки

Cайт соревнования [Гадаем на картах](https://ods.ai/competitions/sberbank-sirius-lesson)
