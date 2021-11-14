Fuzzyness 
===

Raw implementation of SQL 'LIKE' conditions with fuzzyness

Dependency
--
* none

Usage
--

```js
let rawValue = 'with eror';
let cond = new Fuzzyness('field_name', rawValue, 2);
console.log('SELECT * FROM table '+cond.get());
```

API Doc
--
```js
Fuzzyness(pField, pValue, pCount = 2)
```

|Name   |Type  |Description                           |
|-------|------|--------------------------------------|
|`pField`|String|Field name                            |
|`pValue`|String|Value to mess with                    |
|`pCount`|Number|Number of incorrect chars             |

Todo
--
- [ ] Escape special char
- [ ] Multiple fields support