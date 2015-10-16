# Темы проектов лаборатории LAMBDA HSE для студентов 

## MLBOX (универсальный классификатор)	

Имеется набор оберток для различных библиотек машинного обучения. Обертки написаны на питоне и обладают одинаковым интерфейсом. 

Необходимо дать возможность исследователям использовать классификаторы из других языков (Lua, R, Ruby, ...) под различными операционными системами. 

Для этого к упакованным в docker-контейнер алгоритмам надо написать универсальную обертку, которая сможет ставить задачи на обучение/предсказание в контейнер при помощи запросов. Внутри контейнера единый клиент на питоне должени принимать и обрабатывать запросы. 

Наобходимые навыки: python, scikit-learn, пригодятся навыки асинхронного веб-программирования.

Полугодовой проект

## Нейроинформатика (анализ ЭЭГ)

Совместный проект с группой Алексея Осадчего.

Анализ данных ЭЭГ с целью выделения высокоуровневых паттернов состояния оператора. По данным электроэнцефалограммы надо научиться угадывать задуманное дествие оператора.   

Необходимые навыки: python, scipy stack, sklearn.

Очень близкая задача: https://www.kaggle.com/c/grasp-and-lift-eeg-detection

Годовой проект.

## Gradient reversal for MC/real data calibration, 

Применение доменной адаптации при помощи нейросетей с инверсией градиента к фильтрации событий в физике высоких энергий.	Получить нейросеть, приводящую реальные и смоделированные события в эксперименте LHCb к форме, позволяющей различить физические параметры, но не позволяющей отличить реальные от смоделированных.

Ссылки

1. http://arxiv.org/pdf/1409.7495.pdf	
2. https://www.kaggle.com/c/flavours-of-physics	

План работы

1. Научиться применять нейросети к классификации событий (код можно взять с Kaggle)
2. Реализовать код для обращения градиента
3. Применить сеть с обращением градиента, оценить соответствие полученного представления данных заявленным целям - например, попробовать разделить сигнал шум и смоделированные/реальные данные классификатором."	Полгода (если будут работать как в ШАДе)


## SHiP Tracker

Распознавание тракторий частиц распадов детектора SHiP.	Предлагается улучшить алгоритм восстановления треков заряженных частиц их характеристик по выходным данным детектора	Монте-Карло.	

Базовое решение: https://cds.cern.ch/record/2005715/files/main.pdf	
[Презентация проекта](https://github.com/yandexdataschool/students_projects_2015/raw/master/SHiP_Tracker_HSE.pdf)

План работы:

1. Реализовать линейную регрессию, учитывающую растояния от хитов до проволок + базовое решение; 
2. Новая линейная регрессия + фильтр Калмана.  	

Годовой проект


## CRAYFIS hot-pixel removal/callibration	

Предлагается разработать алгоритм калибровки камеры телефона как детектора космического излучения.

Данные: Rad226 dataset, возможно muon studies	

Ссылки:

1. [презентация проекта](https://github.com/yandexdataschool/students_projects_2015/raw/master/CRAYFIS-LAMBDA.pdf)
2. http://arxiv.org/pdf/1410.2895v1.pdf

Предлагается использовать EM-based KS hot-pixel removal.

Полугодовой проект. 

## CRAYFIS efficient shower detection	

Разработать алгоритм распознование вторичных ливней от частиц ультра высоких энергий.

Доступны симулированные данные. 

Предлагаемые средства для реализации:
Likelihood Maximization	Spark MLLib + Elasticsearch / sklearn / caffe	

1. [презентация проекта](https://github.com/yandexdataschool/students_projects_2015/raw/master/CRAYFIS-LAMBDA.pdf)
2. http://arxiv.org/pdf/1410.2895v1.pdf

Полугодовой проект.


## SkyGrid economics

Моделирование планировщика распределенных задач с учётом рыночной модели облачных вычислений.	Надо исследовать существующие алгоритмы планирования выполнения задач в распределенных системах, построить модель выполнения задач при условии учета стоимости ресурсов для их выполнения и провести моделирование для изучения свойств этой модели

Имеется статистика выполнения задач в skygrid, которую надо использовать.

Ссылки:

1. http://barbie.uta.edu/~hdfeng/CloudComputing/cloud/cloud16.pdf
2. http://www.researchgate.net/publication/235953507_Online_cost-efficient_scheduling_of_deadline-constrained_workloads_on_hybrid_clouds

## Распознавание спутниковых изображений	

Разработка библиотеки алгоритмов удаления типичных артефактов со спутниковых изображений земной поверхности, необходимо разработать и протестировать алгоритмы удаления артефактов со спутниковых сников. 

Интегрировать реализованные алгоритмы в облачную модель выполнения Helix Nebula	спутниковые снимки ESA	-	scikit-image	

Годовой проект.


## Определение типа частицы по отклику детектора (доступно с января)	

Предлагается разработать систему определения типа частицы по откликам разных субдетекторов.
Необходимые навыки: C++, python, sklearn.			

[Презентация проекта](https://github.com/yandexdataschool/students_projects_2015/raw/master/LHCB_tracking_and_pid.pdf)

Годовой проект.
