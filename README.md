# Cafe & Wifi API

Навчальний проєкт із курсу Python — REST API для бази кав'ярень (пошук за локацією, фільтр за наявністю wifi/розеток/туалету, ціна кави тощо).

## Технології

- Python
- Flask
- Flask-SQLAlchemy
- SQLite
- Postman (тестування API та документація)

## Роути API

| Метод | Роут | Опис |
|---|---|---|
| GET | `/random` | Випадкова кав'ярня |
| GET | `/all` | Усі кав'ярні |
| GET | `/search?loc=<location>` | Пошук кав'ярень за локацією |
| POST | `/add` | Додати нову кав'ярню |
| PATCH | `/update-price/<cafe_id>?new_price=<price>` | Оновити ціну кави |
| DELETE | `/report-closed/<cafe_id>?api-key=<key>` | Видалити кав'ярню (потрібен api-key) |

## Документація API

Повна документація з прикладами запитів опублікована в Postman:
https://documenter.getpostman.com/view/42581230/2sBYAxQq5h

## Запуск локально

```bash
pip3 install -r requirements.txt
python3 main.py
```

Сервер запуститься на `http://127.0.0.1:5001`.
