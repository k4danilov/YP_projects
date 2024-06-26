Интернет-магазин «Викишоп» запускает новый сервис. Теперь пользователи могут редактировать и дополнять описания товаров, как в вики-сообществах. То есть клиенты предлагают свои правки и комментируют изменения других. Магазину нужен инструмент, который будет искать токсичные комментарии и отправлять их на модерацию. 
В распоряжении набор данных с разметкой о токсичности правок.

**Цель проекта:**
- Обучить модель классифицировать комментарии на позитивные и негативные. Метрика качества *F1* должна быть не меньше 0.75

**Результаты**
В ходе работы на проектом выполнены следующие мероприятия:
- Загружены и проанализированы описания товаров в интернет-магазине Wikishop.
- Подготовлены данные для обучения моделей: произведены лемматизация и токенизация описаний, данные разделены на обучающую и тестовую выборки с использованием стратификации.
- Обучены 3 разные модели (LinearRegression, RandomForest, LightGBM), подобраны оптимальные гиперпараметры. 
- Выбрана наилучшая модель по метрике f1. Ей оказалась модель LightGBM. При проверке качества модели на тестовой выборке метрика f1-score составил 0.79, что входит в пределы порогового значения >0.75.

**Инструменты и техники:** Pandas, sklearn, numpy, NLTK, LightGBM, CatBoost, ML, cross-validation, stemming, feature engineering, word2vec, pipeline
