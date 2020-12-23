# Junta-Project

**VK API GROUP FUNCTIONS.ipynb** — функции для работы с API ВКонтакте, для парсинга групп и пабликов.

* group_wall_post_texts () — сбор тектов постов со стены паблика
* agg_group_member_ids () — сбор подписчиков паблика
* gender_counts () — подсчёт мужчин и женщин среди подписчиков паблика
* param_counts (bdate/ city/ country/ home_town) — выявление года рождения, города, страны и родного города подписчиков паблика и подсчёт этих показателей

**ХУНТА Рабочий файл (хаотичный).ipynb** — мой сбор данных по пабликам "Хунта Экспресс", "Балканский Экспресс" и "Она развалилась". Может пригодиться лишь как подсказка, а не как полноценный рабочий файл, потому что я его не очищала от мусора, очень грязный код в попытках найти истину. Кроме того, данные, которые я парсила в этом файле, настолько большие по объёму, что любой неудачный шаг может перегрузить оперативную память компьютера, и Jupyter Notebook перестанет отвечать. Поэтому я выставляю этот файл в исходном, рабочем виде, а не переделываю его начисто, потому что рискую потерять всё. Лучше синица в руках, чем журавль в небе.

Как бы то ни было, в результате работы этого кода получилось выявить главное — ядро, пересечение аудиторий всех трёх пабликов. Его мы и анализировали в следующих ноутбуках.

На картинке это ядро по центру. Центр левого ёжика — паблик "Она развалилась", центр правого ёжика — "Хунта Экспресс", центр нижнего — "Балканский Экспресс". Шапочки вокруг центров — это подписчики, которые подписаны исключительно на этот паблик, но не подписаны на другие.
![](https://sun9-29.userapi.com/impg/on-JeRXokrqrdCPce5UcP3Fi-EDSExTJYkSzVw/EuOqiQE4XIg.jpg?size=1024x1024&quality=96&proxy=1&sign=e0157b3bc76c29a769f64c986debf1dc&type=album)

**ХУНТА Описательная статистика.ipynb** — применение функций из файла VK API GROUP FUNCTIONS.ipynb для анализа полученного ядра. Выводы про пол, возраст и регионы подписчиков. 

**ХУНТА Communities Clear.ipynb** — применение communities detection. Выявление крупнейшего сообщества в рамках ядра и анализ интересов этого сообщества через парсинг пабликов и групп этого ядра.
