# income_prediction
Предсказание дохода лиц на основе признаков (образование, семейный статус, прирост капитала и т.д.). Задание на тему: "Классификация: Логистическая регрессия и SVM"

1. Загрузила данные. Импортировала данные из файла csv и отобразила в виде датафрейма с помощью pandas.
2. Предобработала данные. Удалила пропуски данных с "?".
3. Визуализировала данные (взяла один признак для примера). Отобразила на графике heatmap (тепловая карта) зависимость дохода от образования с помщью инструментала seaborn.
4. Преобразовала признаки из категориальной формы в числовую для дальнейшего построениря модели. Использовала one-hot encoding и функцию get_dummies для преобразования признаков X и кодировщик LabelEncoder – для целевой переменной.
5. Предсказала доход с помощью алгоритма логистической регрессии. Модель распределила лиц по двум классам. Предварительно потребовалась стандартизация данных с помощью StandardScaler. Его и LogisticRegression одновременно помог выполнить pipeline.
6. Предсказала вероятность принадлежности человека к каждому из классов с помощью predict_proba.
7. Проверила точность модели с помощью метода score. Показатель для тестовой выборки превысил 0,79.
8. Кроме логистической регрессии, построила модель SVM. Она показала результат лучше – 0,80.
