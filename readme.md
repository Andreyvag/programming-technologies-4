# Лабораторная работа №4
_Анализ и визуализация данных в Python_

Цель работы — знакомство с средствами анализа данных в Python с использованием интерактивных блокнотов Jupyter.

__Содержание:__
1. [Подготовка](#1-подготовка)
2. [Задание](#2-задание)
3. [Индивидуальное задание](#3-индивидуальное-задание)

## 1. Подготовка
Для выполнения работы понадобятся Python 3, Jupyter и библиотеки pandas, matplotlib и scikit-learn. Есть несколько способов подготовить рабочее окружение, некоторые из них перечислены ниже.

### 1.1 Способ для ленивых: [Google Colab](https://colab.research.google.com)
Просто переходите на сайт и сразу можете приступать к написанию кода.

### 1.2 Способ для тех, кому не жалко места: [Anaconda](https://www.anaconda.com/products/individual#Downloads)
Anaconda — это всё, что вам нужно и даже больше, собранное в один  установочный пакет. После установки в системе появится приложение Jupyter Notebooks, после запуска которого у вас появится создать возможность блокнот в свежеоткрывшемся окне браузера.

### 1.3 Способ для тех, кому жалко места: [Miniconda](https://docs.conda.io/en/latest/miniconda.html)
Miniconda не тянет с собой все пакеты, но требует от вас некоторых телодвижений:
```bash
conda activate base
conda install jupyter pandas matplotlib scikit-learn
jupyter notebook
```

Это не все возможные способы добиться желаемого, но самые простые.

## 2. Задание
1. Открыть интерактивный блокнот `lab4.ipynb` в Jupyter и ознакомиться с материалами.
2. Определить долю выживших и определите 2 наиболее важных признака для выживания при помощи `DecisionTreeСlassifier` на основе данных из `datasets/titanic.csv`.
3. Для задачи о классификации вина методом ближайших соседей произведите масштабирование признаков с помощью функции `sklearn.preprocessing.scale`. Снова найдите оптимальное k на кросс-валидации. Помогло ли масштабирование?
4. Для данных `europe.csv` постройте модель зависимости качества жизни (Life.expect) от остальных факторов, исключая название страны. Используя метрику `r2_score`, оцените качество построенной модели.

## 3. Индивидуальное задание
1. Определите самое распространённое женское имя среди пассажиров Титаника. Извлеките из полного имени пассажира (колонка Name) его личное имя. Попробуйте вручную разобрать несколько значений столбца Name и выработать правило для извлечения имен, а также разделения их на женские и мужские.
