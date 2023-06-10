# Выполнение работы по дисциплине "Нейроэволюционные вычисления" по направлению 09.04.01 "Информатика и вычислительная техника" в НИ ТПУ.

## Требуемые модули для запуска
Для запуска программы необходима установка следующих модулей на Python: 
* networkx; 
* matplotlib; 
* pandas;
* neat-python;
* numpy;
* graphviz;
* pygraphviz.

## Об алгоритме NEAT
Прочитать об алгоритме NEAT можно в  журнальной статье создателя этого алгоритма <a href="[Lessons/HTML/Practice.html](https://nn.cs.utexas.edu/downloads/papers/stanley.ec02.pdf)">по этой ссылке</a>.

## Описание программы
Программа записана в файле с разрешением .ipynb и включает в себя следующие функции:
* загрузка данных из датасета и конфигурационного файла (для работы NEAT);
* расчёт фитнес-функции;
* построение графа нейронной сети;
* расчёт метрик;
* сохранение результатов в файл.

## Запуск программы
Установка необходимых модулей.
Запуск ipynb-файла, представленного в этом репозитории.
В случае необходимости изменения параметров алгоритма NEAT, необходимо изменить конфигурационный файл, представленный в этом репозитории.

## Описание датасета
Для работы алгоритма NEAT использован 1.	Heart Attack Analysis & Prediction Dataset, который представлен на сайте <a href="https://www.kaggle.com/datasets/rashikrahmanpritom/heart-attack-analysis-prediction-dataset">Kaggle</a>. Датасет содержит 303 записи, каждая из которых содержит 13 признаков и 1 целевую переменную. Однако, во избежание чрезмерной изменчивости фенотипов особей в ходе работы алгоритма, набор данных был сокращен на 4 признака (trtbps, chol, fbs, rest_ecg) на основании матрицы корреляции по критерию Пирсона (<0.2). Оригинальные признаки:
* Age : Age of the patient
* Sex : Sex of the patient
* exang: exercise induced angina (1 = yes; 0 = no)
* ca: number of major vessels (0-3)
* cp : Chest Pain type chest pain type
* trtbps : resting blood pressure (in mm Hg)
* chol : cholestoral in mg/dl fetched via BMI sensor
* fbs : (fasting blood sugar > 120 mg/dl) (1 = true; 0 = false)
* rest_ecg : resting electrocardiographic results
* thalach : maximum heart rate achieved
* target : 0= less chance of heart attack 1= more chance of heart attack


