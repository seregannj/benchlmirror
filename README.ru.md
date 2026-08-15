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
