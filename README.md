# DLSchool2021-advanced-project
MIPT DLSchool final project for advanced track. A research of different approaches to transfer learning on DeepLabV3

## Цель
Исследовать различные способы адаптации архитектуры DeepLabV3, предобученной на 3-х канальных RGB изображениях из ImageNet для использования дополнительных каналов для задачи семантической сегментации спутниковых изображений.

## Введение
Трансферное обучение является основным подходом к решению новых задач в машинном обучении, так как предобученные модели часто показывают лучшие результаты, чем модели специально созданные под конкретную задачу, даже если они не используют часть имеющихся данных в связи с архитектурными особенностями (https://www.azavea.com/blog/2017/05/30/deep-learning-on-aerial-imagery/).

В этом исследовании я сравниваю следующие техники трансферного обучения:
1. Обучение нижних слоёв на новых каналах с последующей вставкой карт активации в основную модель на различной глубине.
2. Ансамблирование предсказаний моделей, обученных на различных комбинациях каналов, используя геометрическое среднее.
3. Суммирование похожих каналов, для усиления сигнала и замена одного из исходных каналов на усиленный.
4. Сравнение с более простой архитектурой UNet, переписанную под 8 каналов.
5. Сравнение с аугментированными данными.

Отчёт по каждой задаче приведён в соответствующих ноутбуках .ipynb
