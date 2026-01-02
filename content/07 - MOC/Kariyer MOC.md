---
created: 2026-01-01
modified: 2026-01-01
tags: [moc, kariyer, profesyonel]
type: moc
---

# 🎯 Kariyer MOC

> *Profesyonel gelişim, kariyer planlaması ve iş yaşamı hakkındaki notların merkezi.*

## 📋 Kariyer Hedefleri

### Kısa Vadeli (1 yıl)
- [ ] 

### Orta Vadeli (3-5 yıl)
- [ ] 

### Uzun Vadeli (10+ yıl)
- [ ] 

## 🏗️ Beceri Alanları

### Teknik Beceriler
- 

### Soft Skills
- 

### Liderlik
- 

## 📊 Aktif Kariyer Projeleri

```dataview
TABLE status as "Durum", deadline as "Deadline"
FROM "02 - Projects"
WHERE contains(tags, "kariyer")
SORT deadline ASC
```

## 📚 Kariyer Kitapları

```dataview
LIST
FROM "04 - Resources/Kitap Notlari"
WHERE contains(tags, "kariyer") OR contains(tags, "liderlik") OR contains(tags, "iş")
SORT file.name ASC
```

## 💡 Kariyer Notları

```dataview
TABLE tags as "Etiketler", created as "Tarih"
FROM "06 - Zettelkasten"
WHERE contains(tags, "kariyer") OR contains(tags, "profesyonel")
SORT created DESC
LIMIT 15
```

## 🔗 İlgili Alanlar

- [[03 - Areas/Kariyer/]]
- [[Networking Stratejileri]]
- [[CV ve LinkedIn Optimizasyonu]]

---

*"Kariyer bir maraton, sprint değil."*

