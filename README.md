# yamdb

Проект Yamdb

## Что нужно для старта

`python3.9`

## Подготовка к работе

```python
python3.9 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
pre-commit install
```

## Работа с Git

[Git guide](./docs/Commits.md)

## manage.py custom commands
### import
```python
python3 manage.py import Genre
```
or
```python
python3 manage.py import Category Genre Title GenreTitle
```
or
```python
python3 manage.py import Category Genre Title GenreTitle User Review Comment
```
### Few notes:
+ Order is important. For example, Review.author is foreign key field referencing User.id, so we cannot import Review before User

## Создатели

- [Иван Сизов](https://github.com/frrenzy)
- [Кирилл Панов](https://github.com/pankirbor)
- [Олег Призов](https://github.com/OlegPrizov)
