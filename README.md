# JetBrains

1. EDA-были построенны графики распределений стоп слов, первых слов, пунктуаций и других зависимостей
Кстати как видно в разных категориях знаки препинания имеют разные распределения, например % встречался только в тестах связанные с физикой, мб это можно было бы использовать
в future engineering
2. Data Cleaning-очистили от мусора текстовые признаки
3. С помощью TruncatedSVD перевели в размерность 2 , и построили эти точки, как видно tf-idf и countvectorizer примерно одинаково разделяют классы и делают это относительно неплохо, 
обычный Tokenizer сделал это более хуже.
4. С помощью Word2Vec сделали RNN, вроде показало +- неплохое качество, можно конечно улучшить я уверен, но времени не хватило
5. Попробовали с помощью tf-idf разные модели, выдают они хуже чем RNN, поэтому предикты будет делать с помощью RNN
6. feature engineering-Нарисовали распределения количество первыых слов в текстах и первые слова в текстах для разных категорий, как видно из распределний количества слов, они
распределены примерно одинаково поэтому добавление этого признака не даст не выйгрыша и не проигрыша, добавим признак первое слово в тексте, как видно качество стало хуже,поэтому
уберем этот признак.Соотвественно никаких новых признаков мы не добавляем

submission_JetBrains-файл предсказаний
