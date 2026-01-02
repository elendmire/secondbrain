---
uid: 20260101120300
created: 2026-01-01 12:03
modified: 2026-01-01 12:03
tags: [dataview, obsidian, sorgu, araç]
related: [Obsidian Başlangıç Rehberi, Templater Kullanımı]
source: Dataview Documentation
status: evergreen
---

# Dataview ile Dinamik Sorgular

Dataview, Obsidian notlarını sorgulanabilir bir veritabanı gibi kullanmayı sağlayan güçlü bir eklentidir.

## Temel Sorgu Türleri

### LIST
Basit liste görünümü:
```dataview
LIST
FROM "06 - Zettelkasten"
LIMIT 5
```

### TABLE
Tablo görünümü:
```dataview
TABLE tags, created
FROM "06 - Zettelkasten"
SORT created DESC
LIMIT 5
```

### TASK
Görev listesi:
```dataview
TASK
WHERE !completed
LIMIT 10
```

## Sık Kullanılan Sorgular

### Orphan Notlar (Bağlantısız)
```dataview
LIST
WHERE length(file.inlinks) = 0 AND length(file.outlinks) = 0
```

### Son 7 Günde Değiştirilen
```dataview
TABLE file.mtime as "Değiştirilme"
WHERE file.mtime >= date(today) - dur(7 days)
SORT file.mtime DESC
```

### Belirli Tag'e Sahip Notlar
```dataview
LIST
WHERE contains(tags, "pkm")
```

## İpuçları

1. Frontmatter'da tutarlı metadata kullan
2. Inline field'ları kullan: `key:: value`
3. Sorguları MOC'larda kullan
4. Performans için `LIMIT` ekle

---

*Bağlantılar: [[PKM MOC]] | [[Programlama MOC]]*

