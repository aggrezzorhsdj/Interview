## Interface и type
Разница Interface и type
Интерфейс можно использовать при создании классов, type только в качества типа
type:
сможно реализовать алиасы

Интерфейс:
 мерж определений 

| Рекомендации по использованию | Предпочитайте интерфейсы для типов объектов, контрактов классов и публичных API | Используйте псевдонимы типов для объединений, кортежей, примитивов и отображенных типов |
| ------------------------- | -------------------------------------------------------------------- | ----------------------------------------------------------------- |
| | | |
| Расширение/составление типов | Использует ключевое слово `extends` | Использует типы пересечения (`&`) |

# Разница между интерфейсом и абстракным классом

## Дженерики
Что такое, для чего используются
```typescript
interface Foo<T> {
	value: T;
}
```
## Utility Types
Что такое, для чего используют, какие есть utility types
Partial - делает все поля необязательными
Require - делает все поля обязательными
Record<Key, Value> - создает дженериковый тип объекта, тип ключа которого будет key, а значение Value
Omit<T, 'key' | 'key2'> - вычитает поле key, key2 из типа T
Pick<T, 'key' | 'key2'> - извлекает поле key, key2 из типа T

# unknown vs any

- **any** — любой тип, компилятор не проверяет операции с переменной, можно делать что угодно, но это небезопасно и может привести к ошибкам во время выполнения.
    
- **unknown** — нетзвестный  тип, но для использования значения нужно обязательно проверить его тип, что делает код безопаснее и предотвращает ошибки
	- - Компилятор не позволит напрямую обращаться к свойствам или методам переменной unknown без предварительной проверки типа.
	- Однако **переменную типа unknown нельзя присвоить переменной с другим, более конкретным типом без явного приведения или проверки типа**. Например, присвоение unknown в number вызовет ошибку: