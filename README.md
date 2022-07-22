## Итоговый проект курса "Машинное обучение в бизнесе"
Данные: с kaggle - https://www.kaggle.com/datasets/blackmoon/russian-language-toxic-comments

Задача: предсказать по описанию коммента, является ли он токсичным или нет (поле toxic). Бинарная классификация

Используемые признаки:

* comment (text) Преобразования признаков: tfidf
Модель: GradientBoostingClassifier (gbc_pipeline.dill)

Для тестирования модели нужно запусить сервер server.ipynb и отправить запрос из test_request.ipynb

Содержание директорий:

* 'app/data' - содержит данные в формате .csv (labeled)
* 'app/model/' - содержит предобученную модель в формате .dill (gbc_pipeline.dill)
* 'app/split/' - содержит разделенные данные (X_train, X_test, y_train, y_test)
* 'app/' - содержит блокноты Jupyter Noutbook с этапами создания модели классификации
