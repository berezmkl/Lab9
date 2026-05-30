# Lab9 — Техніки тест-дизайну "білої скрині"

## Мета
Ознайомлення з техніками тест-дизайну білої скрині: CFG, цикломатична складність, покриття коду.

## Структура проєкту
- `auth.py` — функція `authenticate_user`
- `test_auth.py` — тести (pytest)
- `requirements.txt` — залежності
- `.github/workflows/ci.yml` — CI/CD пайплайн

## Запуск тестів
```bash
pip install -r requirements.txt
coverage run --branch -m pytest
coverage report -m
```

## Висновки
Було реалізовано повне покриття функції `authenticate_user` за допомогою технік білої скрині:
Statement Coverage, Branch Coverage, Condition Coverage, MC/DC, Path Coverage.
Цикломатична складність функції = 5, що відповідає мінімальній кількості тестів для повного покриття шляхів.