# Streamlit RecSys

## Demo
[Streamlit Cloud]()

## RoadMap Задач

**Далее**
- [ ] Добавить альтернатиную сортировку, ранкинг, по популярности фильма (`popularity`)
- [ ] Добавить `selectbox()` для выбора типа модели и подключить к коду приложения

- [ ] Составить выборку с оценками фильмов пользователями (добавить загрузку данных по ссылке и адаптировать к новой структуре)
- [ ] GitHub репозиторий проекта, с последующим merge request от каждого студента
- [ ] Добавить идентификацию пользователей (своя реализация или `streamlit credentials`)
- [ ] Сохранять выбор пользователя (`user_login`, `user_password`, `added_movies`)
- [ ] Сохранять рейтинг выбранных пользователем фильмов (`st.slider` или `st.number_input`)
- [ ] Модель на основе предпочтений пользователей (по списку фильмов, после и по рейтингу)
- [ ] Деплой приложения в облачный сервис (streamlit-hub, hf spaces, heroku)

---
**Если успеем**
- [ ] Добавить метрики качества рекомендаций для модели по пользователям
- [ ] ФидБек рекомендаций от пользователей
- [ ] A/B тестирование на пользователях (сами сделаем или попросим студентов)

---
**Реализовано**
- [x] Исправить проблему со ссылками на постеры
- [x] Базовая модель коллаборативной фильтрации с простой сортировкой, ранкингом, по `cos_sim score`
- [x] Исправить проблему с выводом выбранных фильмов в рекомендациях модели

## GitHub Workflow
1. Fork репозитория https://github.com/valeriylo/RecSys_ML_ASU в свой аккаунт (кнопка Fork в правом верхнем углу)
2. Склонировать свой репозиторий на локальную машину командой `git clone` (предварительно установив `git`)
3. Выбрать ветку `students` командой `git checkout students` или в IDE выбрать нужную ветку
4. Инициализировать виртуальное окружение командой `python -m venv venv` (предварительно установив `python`)
5. Активировать виртуальное окружение командой `source venv/bin/activate` (для Windows `source venv/Scripts/activate`)
6. Установить зависимости командой `pip install -r requirements.txt`
6.1. Создать общий датафрейм, исполнив все ячейки в jupyter ноутбуке `notebooks/process_data.ipynb`
7. Внеся изменения в код, добавить их в индекс командой `git add <file_name>` или в IDE выбрать нужные файлы
8. Сделать коммит изменений командой `git commit -m "commit message"` или в IDE указать комментарий
9. Отправить изменения в свой репозиторий командой `git push origin students` или в IDE выбрать нужную ветку
10. В своем репозитории на GitHub создать Merge Request в ветку `students` репозитория
11. После слияния изменений в ветку `students` основного репозитория, сделать `git pull origin students` или в IDE обновить ветку
12. Повторять шаги 7-11


## Prerequisite

- Python 3.8+

## Installation

```
pip install -r requirements.txt
```

## How to Run App locally

```
streamlit run main.py
```
