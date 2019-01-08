# Этап 2. Проработка моделей данных

## Критерии достижения:

1. Созданы модели и их дополнительные методы.

## Порядок выполнения

1. Создать модели:
    1. Shop
        - name
        - url
        - filename
    2. Category
        - shops (m2m)
        - name
    3. Product
        - category
        - name
    4. ProductInfo
        - product
        - shop
        - quantity
        - price1
        - price2
    5. Order
        - user
        - dt
        - status
    6. OrderItem
        - order
        - product
        - shop
        - quantity
    7. Contact
        - type
        - user
        - value

2. Добавить методы в модели
    1. Product
        - get_info
    2. OrderItem
        - price (property)
        - sum (property)
    3. Contact
        - get_user_contacts (classmethod)
           