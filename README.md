# Export finds a way... through Kyrgyzstan?
Поговорим об ограничении экспорта на бумаге и на деле. После февраля 2022 года можно было заметить много заявлений об уходе компаний из России и ограничении экспорта из многих европейских (и не только) стран. Но что-то подсказывает, что в нашем capital-driven society такой привлекательный рынок многим дороже, чем моральные установки. Надо выяснять кому!

В данном проекте используются датасеты UN Comtrade Database, ежемесячный экспорт из выбранного списка стран в одну конкретную (Россию, Кыргызстан или Казахстан) за 2022 и 2023 года. Рядом с каждым поялением файлов в коде указан год и страна назначения. Все csv файлы можно найти в папке data.

Карты были сделаны при использовании folium, который почему-то любит на гитхабе не открываться. Для полного экспириенса оставляю ссылку на nbviewer, который фиксит проблему с картами (мне очень понравился выбранный геодатасет, и я забыла, что с folium такие проблемы иногда)

https://nbviewer.org/github/kefirahhla/export_finds_a_way/blob/main/export_finds_a_way_main.ipynb

Проект разделен на 5 частей, не считая лирического заключения. В начале каждой части можно найти более подробное описание целей, процесса и методов.
### Часть 1. 
Поиск изначальной информации о импорте в Россию за 2022 и 2023 года. Задача -- выбрать пару стран, экспорт которых в Россию вырос -- и посмотреть, как они импортируют.
### Часть 2. 
Сбор и обработка информации об импорте выбранных стран за 2022 и 2023 года. Чистка столбцов, приведение колонок в порядок, соединение датасетов.
### Часть 3.
Витуализация попарно Кыргызстана и Казахстана с Россией двумя способами. Группировка по странам, boxplots, обычные линии со сглаживанием.
### Часть 4.
Визуализация и сбор коэффициентов линейной регрессии. Посмотрим на тренд экспорта выбранных стран в Кыргызстан, Казахстан и Россию.
### Часть 5.
Геоданные. Наносим собранные коэффициенты на карту и любуемся. Не забываем проверить, как названы страны в выбранном датасете!



