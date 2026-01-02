---
created: 2026-01-01
modified: 2026-01-01
tags: [python, snippet, kod]
type: resource
---

# 🐍 Python Sık Kullanılan Snippet'ler

## Dosya İşlemleri

### Dosya Okuma
```python
with open('dosya.txt', 'r', encoding='utf-8') as f:
    content = f.read()
```

### JSON Okuma/Yazma
```python
import json

# Okuma
with open('data.json', 'r') as f:
    data = json.load(f)

# Yazma
with open('data.json', 'w') as f:
    json.dump(data, f, indent=2, ensure_ascii=False)
```

## List Comprehension

```python
# Basit
squares = [x**2 for x in range(10)]

# Filtreleme ile
evens = [x for x in range(20) if x % 2 == 0]

# Nested
matrix = [[i*j for j in range(5)] for i in range(5)]
```

## Dictionary İşlemleri

```python
# Dict comprehension
squared_dict = {x: x**2 for x in range(5)}

# Merge (Python 3.9+)
merged = dict1 | dict2

# Get with default
value = my_dict.get('key', 'default_value')
```

## Tarih İşlemleri

```python
from datetime import datetime, timedelta

now = datetime.now()
formatted = now.strftime('%Y-%m-%d %H:%M:%S')
parsed = datetime.strptime('2026-01-01', '%Y-%m-%d')
tomorrow = now + timedelta(days=1)
```

## Pandas Temelleri

```python
import pandas as pd

df = pd.read_csv('data.csv')
df.head()
df.describe()
df.groupby('column').mean()
df.to_csv('output.csv', index=False)
```

---

*Bağlantılar: [[Programlama MOC]]*

