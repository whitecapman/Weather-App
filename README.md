# 🛰️ Weather App — Web Application for Weather Forecasts

Интерактивное веб-приложение для просмотра актуального прогноза погоды и визуальных метеокарт, разработанное на **Python** с использованием фреймворка **Streamlit** и API **wttr.in**.

[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.28+-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)](https://streamlit.io/)
[![API](https://img.shields.io/badge/API-wttr.in-blue?style=for-the-badge)](https://github.com/chubin/wttr.in)

👉 **Онлайн-версия приложения:** [weather-app-102.streamlit.app](https://weather-app-102.streamlit.app/)

---

## 📸 Скриншоты интерфейса

<div align="center">
  <h3>Главный экран и карточки метрик</h3>
  <img src="assets/preview_main.png" alt="Главный экран" width="700"/>

  <br/><br/>

  <h3>Графический прогноз погоды</h3>
  <img src="assets/preview_chart.png" alt="Графический прогноз" width="700"/>
</div>

---

## ✨ Ключевые возможности

- **Мультиязычность (i18n):** Поддержка русского, английского (English) и немецкого (Deutsch) языков.
- **Наглядная аналитика:** Вывод ключевых показателей (температура, «ощущается как», вероятность осадков, влажность, скорость ветра, видимость, а также время рассвета и заката в единой метрике).
- **Визуальные карты:** Загрузка и отображение графического PNG-прогноза по требованию.
- **Оптимизация и кэширование:** Использование `@st.cache_data` (TTL = 15 минут) для снижения нагрузки на внешнее API и мгновенной повторной загрузки.
- **Отказоустойчивость:** Обработка ошибок сети, таймаутов, несуществующих городов и резервное переключение ключей локализации API.

---

## 🛠️ Технологический стек

- **Язык программирования:** Python
- **Фреймворк интерфейса:** Streamlit
- **Запросы к API:** Requests
- **Источник данных:** [wttr.in](https://wttr.in) (JSON API + PNG rendering)
