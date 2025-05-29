## Курс Анализ временных рядов методами искусственного интеллекта Весна 2025

[1 Introduction to time series](<./Задание 1/1 introduction_to_time_series_zotov.ipynb>)
Trend, Seasonality, Residuals. Методы разложения временного seasonal_decovpose, STL.
Оценка периода, FFT, plotSpectrum.

[2 Stationarity](<./Задание 2/2 stationarity zotov.ipynb>)
Слабая стационарность. ADF тест (Вннимание! сезонность, гетереоскендатичность). Приведение ряда к стационарному - диффиренцирование, логарифмирование ряда.

[3 Smoothing](<./Задание 3/3 smoothing zotov.ipynb>)
Сглаживание средним, скользящим средним (MA), взвешенным скользящим средним (WMA).
Модели экспоненциального сглаживания (одинарное, двойное, тройное). Предсказание.

[4 AR MA](<./Задание 4/4 ar_ma zotov.ipynb>)
Автокорреляционная функция (ACF) plot_acf. Взаимная корреляция. Косвенная / прямая корреляция. Частичная автокорреляционная функция (PACF) plot_pacf.
Модели авторегресссии (AR), ограничения моделей, определение порядка модели (PACF), удаление тренда и сезонности (diff, ExponentialSmoothing), прогнозирование. Рекомендации по дифференцированию.
Модели скользящего среднего (MA, не путать со сглаживаниеем MA). Определение порядка модели (ACF). Характерные признаки MA модели на графике PACF.

**Упражнения из лекционных блокнотов**

[9 Classification and clustering](<./lecture9/9 classification_clustering zotov.ipynb>)
Метрика, основанная на выравнивании: Dynamic Time Warping (DTW)
DTW algorithm, classification with DTW, clustering with DTW
визуализация классов KernelPCA
Time-series kernels
Time-series embedding (RC - Reservoir Computing)
