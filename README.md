# Cafe & Wifi API

An educational Python project — a REST API for a cafe database (search by location, filter by wifi/sockets/toilet availability, coffee price, etc.).

## Tech stack

- Python
- Flask
- Flask-SQLAlchemy
- SQLite
- Postman (API testing and documentation)

## API routes

| Method | Route | Description |
|---|---|---|
| GET | `/random` | Get a random cafe |
| GET | `/all` | Get all cafes |
| GET | `/search?loc=<location>` | Search cafes by location |
| POST | `/add` | Add a new cafe |
| PATCH | `/update-price/<cafe_id>?new_price=<price>` | Update a cafe's coffee price |
| DELETE | `/report-closed/<cafe_id>?api-key=<key>` | Delete a cafe (requires api-key) |

## API documentation

Full documentation with example requests is published on Postman:
https://documenter.getpostman.com/view/42581230/2sBYAxQq5h

## Running locally

```bash
pip3 install -r requirements.txt
python3 main.py
```

The server runs on `http://127.0.0.1:5001`.
