# NormalSmartDevice 
## Overview
NormlSmartDevice Tool Kit - це сукупність підпрограм, які допомагають створити розумну систему для ідентифікації користувача по фотографії.
Наше АПІ умовно можна поділити на три частини.
### 1. Мікроконтролер ###
Реалізовані засоби для підключення камери до Resbbery Pi, отримання зображення з камери та кодування його в Base64, прередавання даних на сервер за допомогою Rest POST.
### 2. Сервер ###
  Реалізовані засоби для декодування сервером отриманої строки в форматі Base64 назад в jpg зображення, перевірка наявності людини на фотографії в базі даних за допомогою алгоритму розпізнавання та відправка результатів перевірки назад на Resbbery Pi.
### 3. Розпізнавання Лиць ###
Реалізовані засоби для вирізання лиця на фотографії при його наявності, переведення всіх кольорів вхідного зображення в чорно білі,динамічне створення дата сету з людських лиць, тренування моделі на цьому дата сеті за допомогою LBPH алгоритму та визначення подібності взіждного зображення з новим лицем з тренованими моделями.

## NormalSmartDevice Tool Kit Getting Started Guide

Ці документи допоможуть почати роботу з NormalSmartDevice Tool Kit, використати деякі його функції у своєму проекті чи створити NormalSmartDevice власноруч.

NormalSmartDevice Tool Kit містить такі функції:

* [Створення IoT-приладу](iot.md)
* [Відправлення запиту POST з фото на сервер](post.md)
* [Стверення бази даних PostgreSQL](postgresql.md)
* [Заповення бази даних JSON-файлами](json.md)
* [Створення RESTful сервера](server.md)
* [Написання програми для обробки фотографії перед розпізнаванням](crop.md)
* [Створення Дата сету](dataset.md)
* [Створення нейронної мережі для розпізнавання](recognition.md)
