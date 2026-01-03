# 🐍 Python Data Structures – Common Methods & Interview Questions

## 1️⃣ List Methods (mutable, ordered)

| Method         | What it does                                          | Example                                            |
| -------------- | ----------------------------------------------------- | -------------------------------------------------- |
| `append(x)`    | Add element to end                                    | `lst=[1,2]; lst.append(3); print(lst)` → `[1,2,3]` |
| `insert(i, x)` | Insert at index `i`                                   | `lst.insert(1,5); print(lst)` → `[1,5,2,3]`        |
| `remove(x)`    | Remove first occurrence of `x`                        | `lst.remove(5); print(lst)` → `[1,2,3]`            |
| `pop([i])`     | Remove and return element at index `i` (default last) | `lst.pop()` → `3`                                  |
| `index(x)`     | Return first index of `x`                             | `lst.index(2)` → `1`                               |
| `count(x)`     | Count occurrences of `x`                              | `lst.count(2)` → `1`                               |
| `sort()`       | Sort in ascending                                     | `lst.sort(); print(lst)` → `[1,2]`                 |
| `reverse()`    | Reverse list                                          | `lst.reverse(); print(lst)` → `[2,1]`              |
| `copy()`       | Shallow copy                                          | `lst2=lst.copy()`                                  |
| `clear()`      | Remove all elements                                   | `lst.clear(); print(lst)` → `[]`                   |

## 2️⃣ Dictionary Methods (key-value pairs)

| Method                    | What it does                  | Example                                           |
| ------------------------- | ----------------------------- | ------------------------------------------------- |
| `dict.keys()`             | Returns all keys              | `d={"a":1}; print(d.keys())` → `dict_keys(['a'])` |
| `dict.values()`           | Returns all values            | `print(d.values())` → `dict_values([1])`          |
| `dict.items()`            | Returns key-value pairs       | `print(d.items())` → `dict_items([('a',1)])`      |
| `dict.get(key, default)`  | Get value safely              | `d.get('b',0)` → `0`                              |
| `dict.update(other_dict)` | Merge/update dict             | `d.update({'b':2})` → `{'a':1,'b':2}`             |
| `dict.pop(key)`           | Remove and return value       | `d.pop('a')` → `1`                                |
| `dict.popitem()`          | Remove & return last inserted | `d.popitem()`                                     |
| `dict.clear()`            | Remove all items              | `d.clear()`                                       |
| `dict.copy()`             | Shallow copy                  | `d2=d.copy()`                                     |

## 3️⃣ Set Methods (unordered, unique)

| Method                         | What it does                          | Example                                   |        |                  |
| ------------------------------ | ------------------------------------- | ----------------------------------------- | ------ | ---------------- |
| `add(x)`                       | Add element                           | `s={1,2}; s.add(3); print(s)` → `{1,2,3}` |        |                  |
| `remove(x)`                    | Remove element (error if not present) | `s.remove(2); print(s)` → `{1,3}`         |        |                  |
| `discard(x)`                   | Remove element (no error if missing)  | `s.discard(5)`                            |        |                  |
| `pop()`                        | Remove and return arbitrary element   | `s.pop()`                                 |        |                  |
| `clear()`                      | Remove all elements                   | `s.clear()`                               |        |                  |
| `copy()`                       | Shallow copy                          | `s2=s.copy()`                             |        |                  |
| `union()` / `                  | `                                     | Combine sets                              | `{1,2} | {2,3}`→`{1,2,3}` |
| `intersection()` / `&`         | Common elements                       | `{1,2} & {2,3}` → `{2}`                   |        |                  |
| `difference()` / `-`           | Elements in first set only            | `{1,2} - {2,3}` → `{1}`                   |        |                  |
| `symmetric_difference()` / `^` | Elements in either set, not both      | `{1,2} ^ {2,3}` → `{1,3}`                 |        |                  |

💡 Quick Tip: Sets are perfect for finding unique elements, duplicates, or intersections.
