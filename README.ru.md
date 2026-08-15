BenchLM Mirror

<div align="center">🇬🇧 English · 🇷🇺 Русский · 🇨🇳 中文 · 🇪🇸 Español · 🇩🇪 Deutsch · 🇫🇷 Français · 🇯🇵 日本語 · 🇰🇷 한국어

</div>> Автоматически обновляемое зеркало публичных данных BenchLM.



  


---

🎯 Зачем это?

BenchLM предоставляет данные об ИИ-моделях: рейтинги, бенчмарки, цены, скорость и сравнения.

Этот репозиторий создан как простое и удобное зеркало этих данных, которое можно использовать в сторонних проектах.

Что можно делать?

📥 Получать актуальные данные — файлы автоматически обновляются раз в день.

🕐 Отслеживать историю изменений — GitHub сохраняет предыдущие версии файлов.

🔗 Использовать данные напрямую — JSON-файлы доступны через GitHub Raw.

🚀 Подключать данные к своим проектам — для получения JSON не требуется создавать собственный сервер.

📊 Создавать собственные интерфейсы и аналитику на основе данных BenchLM.


Таким образом, репозиторий может использоваться как простой источник данных BenchLM для сайтов, приложений, ботов, аналитических инструментов и других проектов.


---

📊 Данные

Файл	Описание	Raw

models.json	Информация об ИИ-моделях	Открыть
leaderboard.json	Рейтинг моделей	Открыть
benchmarks.json	Информация о бенчмарках	Открыть
pricing.json	Цены на модели	Открыть
speed.json	Скорость и производительность моделей	Открыть
comparisons.json	Сравнения моделей	Открыть



---

🔗 Быстрый доступ

Все данные находятся в директории data/.

GitHub Raw

Например, models.json:

https://raw.githubusercontent.com/seregannj/benchlmirror/main/data/models.json

Другие файлы доступны по аналогичному адресу:

https://raw.githubusercontent.com/seregannj/benchlmirror/main/data/leaderboard.json
https://raw.githubusercontent.com/seregannj/benchlmirror/main/data/benchmarks.json
https://raw.githubusercontent.com/seregannj/benchlmirror/main/data/pricing.json
https://raw.githubusercontent.com/seregannj/benchlmirror/main/data/speed.json
https://raw.githubusercontent.com/seregannj/benchlmirror/main/data/comparisons.json

GitHub API

Файлы также можно получать через GitHub Contents API:

https://api.github.com/repos/seregannj/benchlmirror/contents/data/models.json

> ⚠️ При использовании GitHub API учитывайте ограничения и условия использования GitHub API.




---

💻 Использование

Python

import requests

url = "https://raw.githubusercontent.com/seregannj/benchlmirror/main/data/models.json"

response = requests.get(url)
response.raise_for_status()

data = response.json()

print(data)

JavaScript

const response = await fetch(
  "https://raw.githubusercontent.com/seregannj/benchlmirror/main/data/models.json"
);

if (!response.ok) {
  throw new Error(`HTTP ${response.status}`);
}

const data = await response.json();

console.log(data);

cURL

curl -L https://raw.githubusercontent.com/seregannj/benchlmirror/main/data/models.json


---

🔄 Автоматическое обновление

Данные автоматически загружаются с BenchLM раз в день с помощью GitHub Actions.

Процесс обновления:

BenchLM
   ↓
Загрузка JSON
   ↓
Проверка файла
   ↓
Проверка JSON
   ↓
data/
   ↓
Git commit

Если загрузка файла не удалась, предыдущая версия файла не заменяется.

Обновление также можно запустить вручную через вкладку Actions.


---

🕐 История изменений

Все изменения файлов сохраняются в истории Git.

Это позволяет:

просматривать предыдущие версии данных;

сравнивать изменения между обновлениями;

отслеживать изменения рейтингов, цен и других данных;

восстанавливать предыдущую версию файла при необходимости.


История изменений доступна во вкладке Commits репозитория.


---

📁 Структура

benchlmirror/
│
├── data/
│   ├── models.json
│   ├── leaderboard.json
│   ├── benchmarks.json
│   ├── pricing.json
│   ├── speed.json
│   └── comparisons.json
│
├── .github/
│   └── workflows/
│
├── LICENSE
├── README.md
└── README.ru.md


---

🔗 Источник

Источник данных:

BenchLM

Этот репозиторий является независимым зеркалом и не связан с BenchLM напрямую.


---

⚖️ Лицензия и данные

Код и конфигурация данного репозитория распространяются под MIT License.

Зеркалируемые данные принадлежат их первоначальному источнику.

MIT License не распространяется автоматически на данные BenchLM.

Перед использованием данных ознакомьтесь с условиями и требованиями их первоначального источника.


---

<div align="center">Data from BenchLM

BenchLM · GitHub · Источник данных

</div>
