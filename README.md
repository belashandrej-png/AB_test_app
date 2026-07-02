#  A/B Testing Academy

<div align="center">

![A/B Testing](https://img.shields.io/badge/A%2FB-Testing-blue?style=for-the-badge)
![Status](https://img.shields.io/badge/status-active-success?style=for-the-badge)
![License](https://img.shields.io/badge/license-MIT-green?style=for-the-badge)

**Полный курс по A/B тестированию с интерактивным глоссарием**

[Демо](#) • [Документация](#) • [Глоссарий](#)

</div>

---

##  О проекте

**A/B Testing Academy** — это образовательная платформа, которая предоставляет comprehensive материалы по A/B тестированию, статистическому анализу и оптимизации конверсий.

###  Возможности

-  **Полный курс** по A/B тестированию от основ до продвинутых техник
-  **Интерактивный глоссарий** с определениями всех ключевых терминов
-  **Практические примеры** и кейсы из реальной практики
-  **Статистические методы** анализа результатов тестов
-  **Инструменты и шаблоны** для проведения тестов

###  Для кого этот курс

- Product Managers
- Data Analysts
- Маркетологи
- UX/UI Дизайнеры
- Разработчики
- Предприниматели

---

##  Структура проекта

AB-Testing-Academy/
├── index.html # Главная страница курса
├── glossary.html # Глоссарий терминов
├── assets/
│ ├── css/
│ │ └── style.css # Основные стили
│ ├── js/
│ │ └── main.js # JavaScript функционал
│ └── images/ # Изображения проекта
├── docs/
│ └── methodology.md # Методология тестирования
├── README.md # Этот файл
└── LICENSE # Лицензия проекта


---

##  Быстрый старт

### Вариант 1: Локальный запуск

1. **Склонируйте репозиторий:**
```bash
git clone https://github.com/yourusername/AB-Testing-Academy.git
cd AB-Testing-Academy

2. **Откройте файл в браузере:**

# Просто откройте index.html в любом браузере
# Или используйте локальный сервер:

# Python 3
python -m http.server 8000

# Node.js (если установлен http-server)
npx http-server -p 8000

3. **Перейдите по адресу:**

http://localhost:8000

Вариант 2: GitHub Pages
Проект автоматически публикуется на GitHub Pages по адресу:

https://yourusername.github.io/AB-Testing-Academy

 Содержание курса
Модуль 1: Основы A/B тестирования
Что такое A/B тестирование
Когда проводить тесты
Постановка гипотез
Выбор метрик
Модуль 2: Статистические основы
Статистическая значимость
Размер выборки
P-value и доверительные интервалы
Ошибки I и II рода
Модуль 3: Дизайн эксперимента
Randomization
Сегментация аудитории
Duration теста
AA тесты
Модуль 4: Анализ результатов
Интерпретация данных
Визуализация результатов
Принятие решений
Документирование
 Глоссарий
Полный список терминов доступен в разделе Глоссарий
Популярные термины:
A/B Test — метод сравнения двух версий продукта
Conversion Rate — процент пользователей, выполнивших целевое действие
Statistical Significance — статистическая значимость результатов
Sample Size — размер выборки для теста
P-value — вероятность получить такие же результаты при нулевой гипотезе
Технологии
HTML5 — семантическая разметка
CSS3 — современное оформление с анимациями
JavaScript (ES6+) — интерактивность
GitHub Pages — хостинг
Chart.js — визуализация данных (опционально)

Примеры использования
Пример 1: Расчет размера выборки

// Формула для расчета минимального размера выборки
n = (Z² * p * (1-p)) / E²

где:
Z — Z-score (1.96 для 95% confidence level)
p — ожидаемая конверсия
E — margin of error

Пример 2: Проверка статистической значимости
Используем Z-test для сравнения конверсий:

from scipy import stats

control_conversion = 0.10
treatment_conversion = 0.12
n_control = 10000
n_treatment = 10000

z_stat, p_value = stats.proportions_ztest(
    [n_treatment * treatment_conversion, n_control * control_conversion],
    [n_treatment, n_control]
)

