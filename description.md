## Описание

Каталог содержит продукты, которые организованы по разным категориям.
У каждого продукта есть имя, необязательное описание, необязательное изображение,
цена и доступность.

Модель `Category` содержит поле name и уникальное поле `slug` (уникальность реализуется
за счет создания индекса).

`Product.category` - A ForeignKey to the Category model. This is a one-to-many
relationship: a product belongs to one category and a category contains
multiple products.

`slug`: The slug for this product to build beautiful URLs.

Use the `prepopulated_fields` attribute to specify fields where
the value is automatically set using the value of other fields.

## To learn detail

1. Slug field
2. Типы полей моделей
3. QuerySet
4. Типы отношений в базе данных (один ко многим, многие ко многим)
5. prepopulated_fields
6. cache-based session engine
7. 