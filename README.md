# Reto-09
Iteradores e Iterables

Implementación del Iterador en el menú.

```python
class OrderIterator:
    def __init__(self, items: list[MenuItem]) -> None:
        self._items = items
        self._index = 0

    def __iter__(self):
        return self

    def __next__(self):
        if self._index < len(self._items):
            item = self._items[self._index]
            self._index += 1
            return item
        else:
            raise StopIteration
```  
