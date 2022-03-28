# YandexPracticum-DataScience
Здесь собраны мои проекты по курсу Data Science от YandexPracticum. Для просмотра проекта нажмите на его название.

# [1.Проект по предсказанию эффективности золотодобычи](https://nbviewer.org/github/Cupetz/YanexPractucum-DataScience/blob/main/%D0%B8%D1%81%D1%85%D0%BE%D0%B4%D0%BD%D1%8B%D0%B5%20%D1%84%D0%B0%D0%B9%D0%BB%D1%8B%20%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%BE%D0%B2/1.%20%D0%9E%D0%B1%D1%83%D1%87%D0%B5%D0%BD%D0%B8%D0%B5%20%D0%BC%D0%BE%D0%B4%D0%B5%D0%BB%D0%B8%20-%20%D0%BF%D1%80%D0%B5%D0%B4%D1%81%D0%BA%D0%B0%D0%B7%D0%B0%D0%BD%D0%B8%D0%B5%20%D1%8D%D1%84%D1%84%D0%B5%D0%BA%D1%82%D0%B8%D0%B2%D0%BD%D0%BE%D1%81%D1%82%D0%B8%20%D0%B7%D0%BE%D0%BB%D0%BE%D1%82%D0%BE%D0%B4%D0%BE%D0%B1%D1%8B%D1%87%D0%B8.ipynb)
- в данном проекте обработана большая база сырых данных о золотодобывающих установках с пропусками, аномальными значениями, большим набором признаков (порядка 80), а так же большой объём технической документации для изучения, чтобы разобраться в ньюансах процессов золотодобычи
- вычленены нужные обучающие и целевые признаки для каждой из двух моделей, проведена предобработка данных и обучены обе требуемые модели
- для обучения моделей о оценки их эффективности была задействована кросс-валидация, применено создание собственной метрики качества через make_score, для подбора оптмальных гиперпараметров задействован метод GridSearch. Для сравнения и поиска наиболее эффективной модели были обучены сразу две - случайного леса и логистической регрессии 
# [2.Проект по определению рисков в нефтедобывающей отрасли](https://nbviewer.org/github/Cupetz/YanexPractucum-DataScience/blob/main/%D0%B8%D1%81%D1%85%D0%BE%D0%B4%D0%BD%D1%8B%D0%B5%20%D1%84%D0%B0%D0%B9%D0%BB%D1%8B%20%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%BE%D0%B2/2.%20%D0%9E%D0%B1%D1%83%D1%87%D0%B5%D0%BD%D0%B8%D0%B5%20%D0%BC%D0%BE%D0%B4%D0%B5%D0%BB%D0%B8%20-%20%D0%B2%D1%8B%D0%B1%D0%BE%D1%80%20%D0%BD%D0%B0%D0%B8%D0%BB%D1%83%D1%87%D1%88%D0%B5%D0%B3%D0%BE%20%D1%80%D0%B5%D0%B3%D0%B8%D0%BE%D0%BD%D0%B0%20%D0%B4%D0%BB%D1%8F%20%D0%B4%D0%BE%D0%B1%D1%8B%D1%87%D0%B8%20%D0%BD%D0%B5%D1%84%D1%82%D0%B8.ipynb)
- в данном проекте нужно было оценить риски при выборе определённого реально существующего региона для организации в нём деятельности по добыче нефти - были даны базы данных 3-х регионов с информацией о кол-ве скважин и их характеристиках (объём залежей нефти в каждой из скважин, цена за баррель нефти), а так же была описана экономика самой компании: за сколько они продают нефть и в каких объёмах, каковы их затраты на развёртывание нефтедобывающих установок в новом регионе, сколько нефтедобывающих установок в 1 регионе они могут разместить и т.п.
- данные были предобработаны и изучены, обучена модель для предсказания самых выгодных для нефтедобывающей деятельности скважин в каждом из регионов, вычислена реальная прибыль на каждой из возможных выборок, оценены риски в каждом из регионов уйти в минус, а так же предсказана потенциальная средняя прибыль в каждом из регионов
- оценка рисков проводилась при помощи метода Booststrap , так же как о ценка возможной средней прибыли. После данной оценки был выбран один регион с самым оптмальным соотношением между рисками и потенциальной прибылью
- # [3.Анализ перспективных платформ игрового рынка](https://nbviewer.org/github/Cupetz/YanexPractucum-DataScience/blob/main/%D0%B8%D1%81%D1%85%D0%BE%D0%B4%D0%BD%D1%8B%D0%B5%20%D1%84%D0%B0%D0%B9%D0%BB%D1%8B%20%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%BE%D0%B2/3.%20%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%BF%D0%B5%D1%80%D1%81%D0%BF%D0%B5%D0%BA%D1%82%D0%B8%D0%B2%D0%BD%D1%8B%D1%85%20%D0%BF%D0%BB%D0%B0%D1%82%D1%84%D0%BE%D1%80%D0%BC%20%D0%B8%D0%B3%D1%80%D0%BE%D0%B2%D0%BE%D0%B3%D0%BE%20%D1%80%D1%8B%D0%BD%D0%BA%D0%B0.ipynb)
- был дан большой датафрейм с данными по платформам и играм для них за последние несколько десятилейтий. нужно было по нему оценить какие платформы сейчас являются самыми перспективными для выпуска игр на них, на что в основном стоит смотреть при определении будущего успеха/провала игры, а так же каков потрет геймеров в разных частях света (игры каких жанров/врзрастных рейтингов и т.п. популярнее всего в определённых частях света - чем отличаются вкусы игрока из Японии и игрока из Северной Америки?)
- так же имела место проверка определённых гипотез (выбор граничной статистической значимости, проведение t-test'ов]
- # [4.Анализ рынка недвижимости](https://nbviewer.org/github/Cupetz/YanexPractucum-DataScience/blob/main/%D0%B8%D1%81%D1%85%D0%BE%D0%B4%D0%BD%D1%8B%D0%B5%20%D1%84%D0%B0%D0%B9%D0%BB%D1%8B%20%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%BE%D0%B2/4.%20%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85%20%D1%80%D1%8B%D0%BD%D0%BA%D0%B0%20%D0%BD%D0%B5%D0%B4%D0%B2%D0%B8%D0%B6%D0%B8%D0%BC%D0%BE%D1%81%D1%82%D0%B8%20-%20%D0%BE%D1%86%D0%B5%D0%BD%D0%BA%D0%B0%20%D1%81%D1%82%D0%BE%D0%B8%D0%BC%D0%BE%D1%81%D1%82%D0%B8%20%D0%BA%D0%B2%D0%B0%D1%80%D1%82%D0%B8%D1%80.ipynb)
- был дан весьма большой и сырой датафрейм (множество пропусков, выбросов, дубликатов) о размещенных объявлениях продающихся квартир. необходимо было оценить какие критерии и насколько сильно влияют на среднюю стоимость квартиры и на её потенциальную продажу
- была выполнена предобработка данных с заполнением всех пропусков, удалением дубликатов и выбросов. построено множество гистограм/матриц корреляции/столбчатых диаграмм/диаграмм рассеивания для ответа на вопросы задания
- # [5. Предсказание оптимального тарифа для пользователя мобильной сети](https://nbviewer.org/github/Cupetz/YanexPractucum-DataScience/blob/main/%D0%B8%D1%81%D1%85%D0%BE%D0%B4%D0%BD%D1%8B%D0%B5%20%D1%84%D0%B0%D0%B9%D0%BB%D1%8B%20%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%BE%D0%B2/5.%20%D0%9E%D0%B1%D1%83%D1%87%D0%B5%D0%BD%D0%B8%D0%B5%20%D0%BC%D0%BE%D0%B4%D0%B5%D0%BB%D0%B8%20-%20%D0%BF%D1%80%D0%B5%D0%B4%D1%81%D0%BA%D0%B0%D0%B7%D0%B0%D0%BD%D0%B8%D0%B5%20%D0%BE%D0%BF%D1%82%D0%B8%D0%BC%D0%B0%D0%BB%D1%8C%D0%BD%D0%BE%D0%B3%D0%BE%20%D1%82%D0%B0%D1%80%D0%B8%D1%84%D0%B0%20%D0%B4%D0%BB%D1%8F%20%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D0%BE%D0%B2%D0%B0%D1%82%D0%B5%D0%BB%D1%8F%20%D0%BC%D0%BE%D0%B1%D0%B8%D0%BB%D1%8C%D0%BD%D0%BE%D0%B9%20%D1%81%D0%B5%D1%82%D0%B8.ipynb)
- по данным о пользователях мобильной сети необходимо было обучить модель, которя с определённой точностью сможет предсказывать какой тариф пользователю лучше всего подойдет
- были рассмотрены модели логистической регрессии, случайного леса и решающего дерева - по итогам проверок на валидационной выборке была выбрана лучшая модель
- дополнительно при помощи DummyClassifier была выполнена проверка модели на вменяемость
- # [6. Предсказание уйдёт ли клиент банка](https://nbviewer.org/github/Cupetz/YanexPractucum-DataScience/blob/main/%D0%B8%D1%81%D1%85%D0%BE%D0%B4%D0%BD%D1%8B%D0%B5%20%D1%84%D0%B0%D0%B9%D0%BB%D1%8B%20%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%BE%D0%B2/6.%20%D0%9E%D0%B1%D1%83%D1%87%D0%B5%D0%BD%D0%B8%D0%B5%20%D0%BC%D0%BE%D0%B4%D0%B5%D0%BB%D0%B8%20-%20%D0%BF%D1%80%D0%B5%D0%B4%D1%81%D0%BA%D0%B0%D0%B7%D0%B0%D0%BD%D0%B8%D0%B5%20%D1%83%D0%B9%D0%B4%D1%91%D1%82%20%D0%BB%D0%B8%20%D0%BA%D0%BB%D0%B8%D0%B5%D0%BD%D1%82%20%D0%B1%D0%B0%D0%BD%D0%BA%D0%B0.ipynb)
- по датафрейму с информацией о клиентах банка нужно было предсказать и обучить модель, которая с определённой точностью будет предсказывать будет ли клиент уходить или продолжать сотрудничать с банком в дальнейшем
- было применено масштабирование для того, чтобы приравнять значимость всех признаков, а так же устанён дисбаланс классов, понижающий точность предсказаний
- был применен перевод категориальных параметров в численные для избежания дамми-ловушки (ohe)
- по итогам была получена модель с необходимой точностью предсказаний (метркиами качества в проекте служили f1-мера и auc-roc кривая)
- # [7. Анализ вероятности выплаты кредита](https://nbviewer.org/github/Cupetz/YanexPractucum-DataScience/blob/main/%D0%B8%D1%81%D1%85%D0%BE%D0%B4%D0%BD%D1%8B%D0%B5%20%D1%84%D0%B0%D0%B9%D0%BB%D1%8B%20%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%BE%D0%B2/7.%20%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B2%D0%B5%D1%80%D0%BE%D1%8F%D1%82%D0%BD%D0%BE%D1%81%D1%82%D0%B8%20%D0%B2%D1%8B%D0%BF%D0%BB%D0%B0%D1%82%D1%8B%20%D0%BA%D1%80%D0%B5%D0%B4%D0%B8%D1%82%D0%B0.ipynb)
- один из моих первых проектов ещё без использования методов машинного обучения - по довольно небольшим сырым данным о клиентах банка нужно было устранить все пропуски, выбросы, дубликаты, применить категоризацию данных (в том числе и лемматизацию), чтобы по итогу построить информативную сводную таблицу для определения какие клиенты вероятнее всего будут гасить кредит в срок, а какие просрочат (например погасит ли безработный 40-летний мужчина кредит с большей вероятностью, чем многодетная одинокая мать, но с большим стажем работы?)
- # [8. Анализ данных о пользователях мобильной сети](https://nbviewer.org/github/Cupetz/YanexPractucum-DataScience/blob/main/%D0%B8%D1%81%D1%85%D0%BE%D0%B4%D0%BD%D1%8B%D0%B5%20%D1%84%D0%B0%D0%B9%D0%BB%D1%8B%20%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%BE%D0%B2/8.%20%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85%20%D0%BE%20%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D0%BE%D0%B2%D0%B0%D1%82%D0%B5%D0%BB%D1%8F%D1%85%20%D0%BC%D0%BE%D0%B1%D0%B8%D0%BB%D1%8C%D0%BD%D0%BE%D0%B9%20%D1%81%D0%B5%D1%82%D0%B8%20-%20%D1%81%D1%80%D0%B0%D0%B2%D0%BD%D0%B5%D0%BD%D0%B8%D0%B5%20%D1%82%D0%B0%D1%80%D0%B8%D1%84%D0%BE%D0%B2.ipynb)
- в данном проекте необходимо было вручную посчитать траты всех пользователей по датафрейму клиентов сотового оператора и сравнить клиенты какого тарифа наиболее прибыльны для компании, а какой тариф стоило бы отключить
- представлены объёмные сводные таблицы по проведённым рассчётам, а так же множественные гистограмы, столбатые диаграммы, для представления прибыльности каждой из групп пользователей для компании
- проведена проверка гипотез с определённой граничной статистической значимостью для ответов на ряд вопросов задания 
