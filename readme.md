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

[5 ARMA ARIMA SARIMA](<./Задание 5/5 arma_arima_sarima zotov.ipynb>)
**ARMA**
Разложение на компоненты (trend, seasonality, residual) методы seasonal_decompose, STL.
Замечание про adf тест для синусоиды. adfuller, rolling(window=12).mean(), rolling(window=12).std() для среднемесячной температуры.
Определение сезонности: График автокорреляции, График сезонных подсерий (график по месяцам), График violinplot, Преобразование Фурье.
Устраняем сезонность diff(12).
Определение порядка модели PACF => AR(p), ACF => MA(q). Обучение модели ARMA.
Остатки модели, график acf. Остатки как белый шум, гистограмма, qqplot. Теже графики может воспроизвести обученная модель fit_model.plot_diagnostics().
Статистические тесты остатков. Нормальность: тесты Жарке-Бера и Шапиро-Уилка. Автокорреляция: тест Льюнга-Бокса, тест Дербина-Уолка. Тест на гетероскедастичность.
Прогнозирование.
**ARIMA SARIMA AutoARIMA**
Оценка качества. Ошибка MSE, MAPE. Сложность модели, AIC, BIC (Information Criterion).
Поиск по сетке. EDA. Pipeline выбора параметров.

[6 unit root; hurst](<./Задание 6/6 unit_root_hurst zotov.ipynb>)
**unit root** AR, оператор запаздывания, характеристическое уравнение.
**ADF** Уравнение ADF теста, типы теста ADF - n, c, ct, выбор длины лага.
**Mean Reversion Test** Возврат к среднему значению VS стационарность.
**Показатель Херста ($H$)** Постоянные и антипостоянные временные ряды.
**Броуновское движение** Дисперсия, геометрическое броуновское движение.

[7 signal transforms; filters](<./Задание 7/7 signal_transforms_filters zotov.ipynb>)
**FT** Fourier transform (прямое и обратное)
**DFT** Discrete Fourier transform. fft(y) fftfreq(n,d) fftshift(x)
**Spectral Leakage** $f_s$ sampling frequency. разрешение по основной частоте $1/f_s$. Период сигнала не кратен шагу дискретизации ($\frac{1}{f_s} \nmid \frac{1}{f}$).
**FT свойства** линейность, сдвиг по времени, масштабирование, свёртка, дифференцирование, интегрирование, теорема Парсеваля.
**Фильтры** частотная характеристика, передаточная функция, Диаграмма Боде.
**Фильтры нижних / высоких частот / полосовые** LPF-LowPassFilter, HPF-HighPassFilter, BPF-BandPassFilter, Окно Хана, Фильтр Тьюки, Фильтр Баттерворта.
**Полосовые режекторные фильтры** BSF-BandStopFilter.
**Прогноз с помощью FT**

**Упражнения из лекционных блокнотов**

[9 Classification and clustering](<./lecture9/9 classification_clustering zotov.ipynb>)
Метрика, основанная на выравнивании: Dynamic Time Warping (DTW)
DTW algorithm, classification with DTW, clustering with DTW
визуализация классов KernelPCA
Time-series kernels
Time-series embedding (RC - Reservoir Computing)
