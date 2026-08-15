# BenchLM Mirror

<div align="center">

[🇬🇧](README.md) · 🇷🇺 · [🇨🇳](README.zh.md) · [🇪🇸](README.es.md) · [🇩🇪](README.de.md) · [🇫🇷](README.fr.md) · [🇯🇵](README.ja.md) · [🇰🇷](README.ko.md)

</div>

> Автоматически обновляемое зеркало публичных данных [BenchLM](https://benchlm.ai/).

[![Обновление](https://img.shields.io/badge/обновление-ежедневно-blue?style=for-the-badge)](https://github.com/seregannj/benchlmirror/actions)
[![Источник](https://img.shields.io/badge/источник-BenchLM-black?style=for-the-badge)](https://benchlm.ai/data)
[![Файлы](https://img.shields.io/badge/данные-6%20JSON-green?style=for-the-badge)](./data/)

---

## 🎯 Зачем это?

BenchLM предоставляет полезные данные об ИИ-моделях: рейтинги, бенчмарки, цены, скорость и сравнения.

Этот репозиторий создан как **простое и удобное зеркало этих данных**, которое можно использовать в сторонних проектах.

### Что можно делать?

- 📥 **Получать актуальные данные** — файлы автоматически обновляются раз в день.
- 🕐 **Отслеживать историю изменений** — GitHub сохраняет предыдущие версии файлов.
- 🔗 **Использовать данные напрямую** — JSON-файлы доступны через GitHub Raw.
- 🚀 **Подключать к своим проектам** — не требуется создавать собственный сервер только для получения данных.
- 📊 **Создавать собственные интерфейсы и аналитику** на основе данных BenchLM.

Таким образом, этот репозиторий может использоваться как **простой промежуточный источник данных BenchLM** для сайтов, приложений, ботов, аналитических инструментов и других проектов.

---

## 📊 Данные

| Файл | Описание | Raw |
|:---|:---|:---:|
| [`models.json`](./data/models.json) | Информация об ИИ-моделях | [Открыть](https://raw.githubusercontent.com/seregannj/benchlmirror/main/data/models.json) |
| [`leaderboard.json`](./data/leaderboard.json) | Рейтинг моделей | [Открыть](https://raw.githubusercontent.com/seregannj/benchlmirror/main/data/leaderboard.json) |
| [`benchmarks.json`](./data/benchmarks.json) | Информация о бенчмарках | [Открыть](https://raw.githubusercontent.com/seregannj/benchlmirror/main/data/benchmarks.json) |
| [`pricing.json`](./data/pricing.json) | Цены на модели | [Открыть](https://raw.githubusercontent.com/seregannj/benchlmirror/main/data/pricing.json) |
| [`speed.json`](./data/speed.json) | Скорость и производительность моделей | [Открыть](https://raw.githubusercontent.com/seregannj/benchlmirror/main/data/speed.json) |
| [`comparisons.json`](./data/comparisons.json) | Сравнения моделей | [Открыть](https://raw.githubusercontent.com/seregannj/benchlmirror/main/data/comparisons.json) |

---

## 🔗 Быстрый доступ

Все данные находятся в директории [`data/`](./data/).

### Raw GitHub

Каждый JSON можно получать напрямую:

```text
https://raw.githubusercontent.com/seregannj/benchlmirror/main/data/models.json

Просто замените models.json на нужный файл.

GitHub API

Файлы также можно получать через GitHub Contents API:

https://api.github.com/repos/seregannj/benchlmirror/contents/data/models.json

> ⚠️ При использовании GitHub API учитывайте ограничения GitHub API и условия их использования.




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

Перед заменой существующего файла данные проходят проверку. Если загрузка или проверка неудачна, предыдущая рабочая версия файла сохраняется.

Обновление также можно запустить вручную:

Actions → Daily download from BenchLM → Run workflow


---

🕐 История изменений

Все изменения данных сохраняются в истории Git.

Это позволяет:

просматривать предыдущие версии файлов;

сравнивать изменения между обновлениями;

отслеживать изменения рейтингов, цен и других данных;

при необходимости восстанавливать предыдущую версию.


История доступна во вкладке Commits репозитория.


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
│       └── update.yml
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
```
