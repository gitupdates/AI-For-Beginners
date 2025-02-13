# Моделирование языка

Семантические встраивания, такие как Word2Vec и GloVe, на самом деле являются первым шагом к **моделированию языка** — созданию моделей, которые каким-то образом *понимают* (или *представляют*) природу языка.

## [Предварительный тест](https://red-field-0a6ddfd03.1.azurestaticapps.net/quiz/115)

Основная идея моделирования языка заключается в обучении на неразмеченных наборах данных в неконтролируемом режиме. Это важно, потому что у нас есть огромные объемы неразмеченного текста, в то время как количество размеченного текста всегда будет ограничено тем количеством усилий, которое мы можем потратить на разметку. Чаще всего мы можем строить языковые модели, которые могут **предсказывать пропущенные слова** в тексте, поскольку легко замаскировать случайное слово в тексте и использовать его в качестве обучающего примера.

## Обучение встраиваний

В наших предыдущих примерах мы использовали заранее обученные семантические встраивания, но интересно посмотреть, как эти встраивания могут быть обучены. Существует несколько возможных идей, которые можно использовать:

* **N-граммное** моделирование языка, когда мы предсказываем токен, смотря на N предыдущих токенов (N-грамма)
* **Непрерывный мешок слов** (CBoW), когда мы предсказываем средний токен $W_0$ в последовательности токенов $W_{-N}$, ..., $W_N$.
* **Скип-грамм**, где мы предсказываем набор соседних токенов {$W_{-N},\dots, W_{-1}, W_1,\dots, W_N$} из среднего токена $W_0$.

![изображение из статьи о преобразовании слов в векторы](../../../../../translated_images/example-algorithms-for-converting-words-to-vectors.fbe9207a726922f6f0f5de66427e8a6eda63809356114e28fb1fa5f4a83ebda7.ru.png)

> Изображение из [этой статьи](https://arxiv.org/pdf/1301.3781.pdf)

## ✍️ Примеры ноутбуков: Обучение модели CBoW

Продолжайте свое обучение в следующих ноутбуках:

* [Обучение CBoW Word2Vec с TensorFlow](../../../../../lessons/5-NLP/15-LanguageModeling/CBoW-TF.ipynb)
* [Обучение CBoW Word2Vec с PyTorch](../../../../../lessons/5-NLP/15-LanguageModeling/CBoW-PyTorch.ipynb)

## Заключение

На предыдущем уроке мы увидели, что встраивания слов работают как магия! Теперь мы знаем, что обучение встраиваний слов — это не очень сложная задача, и мы должны быть в состоянии обучить свои собственные встраивания слов для текстов специфичных для домена, если это необходимо.

## [Пост-лекционный тест](https://red-field-0a6ddfd03.1.azurestaticapps.net/quiz/215)

## Обзор и самообучение

* [Официальный учебник PyTorch по моделированию языка](https://pytorch.org/tutorials/beginner/nlp/word_embeddings_tutorial.html).
* [Официальный учебник TensorFlow по обучению модели Word2Vec](https://www.TensorFlow.org/tutorials/text/word2vec).
* Использование фреймворка **gensim** для обучения наиболее распространенных встраиваний за несколько строк кода описано [в этой документации](https://pytorch.org/tutorials/beginner/nlp/word_embeddings_tutorial.html).

## 🚀 [Задание: Обучение модели Skip-Gram](lab/README.md)

В лаборатории мы бросаем вам вызов модифицировать код из этого урока, чтобы обучить модель skip-gram вместо CBoW. [Читать детали](lab/README.md)

**Отказ от ответственности**:  
Этот документ был переведен с использованием услуг машинного перевода на основе ИИ. Хотя мы стремимся к точности, пожалуйста, имейте в виду, что автоматические переводы могут содержать ошибки или неточности. Оригинальный документ на его родном языке следует считать авторитетным источником. Для критически важной информации рекомендуется профессиональный человеческий перевод. Мы не несем ответственности за любые недоразумения или неправильные интерпретации, возникающие в результате использования этого перевода.