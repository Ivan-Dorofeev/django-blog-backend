# Блог

Блог на Django

## Описание

Сайт выводит блоги из базы данных. 
Показывает самые популярные блоги на главной страницы и новые.

![image](https://user-images.githubusercontent.com/58893102/186417641-c7342d8e-f294-4d68-8dbe-319057063e12.png)

Можно подробно посмотреть каждый блог и комментарии с нему.

![image](https://user-images.githubusercontent.com/58893102/186418031-65c3bfc3-1a1a-4e34-8b8f-f9eab34ad04e.png)

В контакты подгружена карта с точными координатами адреса:

![image](https://user-images.githubusercontent.com/58893102/186418169-3a9f14c0-4668-44e6-a433-d2888c65434d.png)


## Запуск

Для запуска блога у вас уже должен быть установлен Python 3.

- Скачайте код
- Установите зависимости командой `pip install -r requirements.txt`
- Запустите сервер командой `python3 manage.py runserver`

После этого переходите по ссылке [127.0.0.1:8000](http://127.0.0.1:8000), вы увидите главную страницу.

## Переменные окружения

Часть настроек проекта берётся из переменных окружения. Чтобы их определить, создайте файл `.env` рядом с `manage.py` и запишите туда данные в таком формате: `ПЕРЕМЕННАЯ=значение`.

**Для запуска проекта эти настройки не требуются**, значения уже проставлены по-умолчанию.

Доступны следующие переменные:
- `DEBUG` — дебаг-режим. Поставьте `True`, чтобы увидеть отладочную информацию в случае ошибки. Выключается значением `False`.
- `SECRET_KEY` — секретный ключ проекта. Например: `erofheronoirenfoernfx49389f43xf3984xf9384`.
- `ALLOWED_HOSTS` — см [документацию Django](https://docs.djangoproject.com/en/3.1/ref/settings/#allowed-hosts).
- `STATIC_URL` — по-умолчанию это `'/static/'`. [Что такое STATIC_URL](https://docs.djangoproject.com/en/3.0/ref/settings/#std:setting-STATIC_URL).
- `STATIC_ROOT` — по-умолчанию это `'None'`, т.е. текущая папка. [Что такое STATIC_ROOT](https://docs.djangoproject.com/en/3.0/ref/settings/#std:setting-STATIC_ROOT).
- `MEDIA_URL` — по-умолчанию это `'/media/'`. [Что такое MEDIA_URL](https://docs.djangoproject.com/en/3.0/ref/settings/#std:setting-MEDIA_URL).
- `MEDIA_ROOT` — по-умолчанию это `'media'`. [Что такое MEDIA_ROOT](https://docs.djangoproject.com/en/3.0/ref/settings/#std:setting-MEDIA_ROOT).


### Контакты

Страница называется `contact`.

Её можно найти по адресу [127.0.0.1:8000/contacts](127.0.0.1:8000/contacts). К шаблонизации в неё отдаётся только переменная `html_map`. Это строка, в которой лежит HTML-код с картой.
