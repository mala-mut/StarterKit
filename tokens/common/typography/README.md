# Как устроена типографика

Предусмотрена расширяемая и гибкая матрица токенов. Если корректно развивать её, в дальнейшем будет легко дотюнивать значения и пакетно накидывать изменения.
Типографика делится на несколько классов с подкатегориями

## Размер

400, 500, 600 и т.д. — отражает размер кегля. 500 — самый ходовой (aka medium), чем больше значение, тем больше кегль

> Почему не майки? Система с числовыми названиями позволяет всегда довольно безболезненно вкрячить новый размер, тогда как между medium и large сложно придумать адекватный неминг

## Стиль

* Display — крупные акцентные стили с компактным интерлиньяжем. Используются в заголовках, для выделения цен и других важных или маркетинговых штук
* Text — текстовые стили для обычного наборного текста
* Compact — текстовые стили для коротких и табличных данных (например, ячеек), имеют более компактный line-height

## Тип

Типы существуют для всех стилей и размеров. По сути это просто классы, которые можно применить к любому тексту

* Accent — выделяющееся начертание (в данном случае, жирное)
* Numeric — начертание с моноширинными цифрами для отображения табличных данных

Могут комбинироваться, например: `text.accent-numeric` — значит текстовый стиль одновременно и жирный, и с моноширинными цифрами