Предложи систему, которая позволит по кропу области с произвольным логотипом на изображении (берется из видео, куда нативно встроена реклама) отвечать на вопрос: "Является ли он логотипом искомой организации?".

В качестве логотипов искомой организации дается несколько образцов. Заранее неизвестно, что именно эта организация будет искаться. Логотипы могут быть текстовыми и нетекстовыми.

На изображении в реальности данные логотипы могут иметь самый различный масштаб, могут иметь отличные характеристики по яркости, контрастности, могут быть повернуты, несколько искажены, иметь небольшие отличия в дизайне.

Из open source датасетов есть такой вариант https://paperswithcode.com/dataset/logodet-3k , если будет полезно.

Мой подход:
1. Обучить CNN на LogoDet-3k
2. Создать свой датасет и применить Аугментацию
3. Проверить работоспособность на реальных фотографиях, где использована нативная реклама
