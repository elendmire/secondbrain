---
uid: 20260101160000
created: 2026-01-01 16:00
modified: 2026-01-01 16:00
tags: [ai, arastirma, agent, sistem, metodoloji]
related: [Research Project - Ana Sayfa, Cursor AI Not Alma]
source: Google AI Co-Scientist
status: evergreen
---

# AI Research Agent Sistemi

Google'ın AI co-scientist sisteminden ilham alarak, Obsidian vault ve Cursor ile multi-agent araştırma sistemi.

## Google AI Co-Scientist Özeti

**Kaynak:** [Google Research Blog](https://research.google/blog/accelerating-scientific-breakthroughs-with-an-ai-co-scientist/)

### Temel Özellikler
- **Multi-agent yapı**: Generation, Reflection, Ranking, Evolution, Proximity, Meta-review
- **Gemini 2.0** tabanlı
- **Test-time compute scaling**: İteratif iyileştirme
- **Self-improvement**: Elo rating sistemi ile otomatik değerlendirme
- **Gerçek dünya validasyonu**: Laboratuvar deneyleri ile doğrulama

### Başarılar
- İlaç yeniden kullanımı (AML için yeni adaylar)
- Hedef keşfi (karaciğer fibrozisi)
- Mekanizma açıklaması (antimikrobiyal direnç)

---

## Bizim Sistem Tasarımı

### Agent Yapısı

| Agent | Rol | Cursor Karşılığı |
|-------|-----|------------------|
| **Supervisor** | Araştırma planı yönetimi | Chat Agent + Composer |
| **Generation** | Hipotez üretimi | Chat Agent (creative mode) |
| **Reflection** | Çıktıları değerlendirme | Chat Agent (critique mode) |
| **Ranking** | Hipotez karşılaştırması | Composer (batch comparison) |
| **Evolution** | İyileştirme döngüleri | Chat Agent (iterative refinement) |
| **Proximity** | Literatür bağlantıları | Codebase search + grep |
| **Meta-review** | Final değerlendirme | Chat Agent (synthesis) |

### Workflow

```
1. Research Goal → Supervisor Agent
2. Supervisor → Generation Agent (hipotez üret)
3. Generation → Reflection Agent (değerlendir)
4. Reflection → Ranking Agent (karşılaştır)
5. Ranking → Evolution Agent (iyileştir)
6. Evolution → Proximity Agent (literatür bağla)
7. Proximity → Meta-review Agent (sentezle)
8. Meta-review → Obsidian'a kaydet
```

---

## Obsidian Entegrasyonu

### Vault Yapısı
- **Research Goals**: `02 - Projects/` veya `03 - Areas/School/Research Project/`
- **Hipotezler**: `06 - Zettelkasten/` (atomik notlar)
- **Literatür**: `04 - Resources/Makale Notlari/`
- **Araştırma Logları**: `01 - Daily/` veya özel klasör

### Dataview Sorguları
- En yüksek puanlı hipotezler
- İşlenmemiş araştırma soruları
- Literatür boşlukları

---

## Kullanım Senaryoları

### Senaryo 1: Yeni Hipotez Üretimi
**Soru:** "WRF modeli ile hard cut-off tahmini nasıl iyileştirilebilir?"

**Süreç:**
1. Supervisor: Araştırma planı oluştur
2. Generation: 5-10 hipotez üret
3. Reflection: Her hipotezi değerlendir
4. Ranking: En umut verici 3'ü seç
5. Evolution: Seçilenleri detaylandır
6. Proximity: Mevcut literatürle bağla
7. Meta-review: Final öneri hazırla

### Senaryo 2: Literatür Boşluğu Analizi
**Soru:** "Türkiye'deki RES hard cut-off çalışmalarında eksik olan nedir?"

**Süreç:**
1. Proximity: Mevcut notları tarar
2. Generation: Potansiyel boşlukları önerir
3. Reflection: Önem sıralaması yapar
4. Meta-review: Araştırma önerileri sunar

---

## Cursor Rules Güncellemesi

`.cursor/rules` dosyasına eklenebilecek:

```markdown
## AI Research Agent Modu

When user requests research assistance:
1. Act as Supervisor Agent: Parse research goal
2. Generate multiple hypotheses (Generation Agent)
3. Evaluate each hypothesis (Reflection Agent)
4. Rank hypotheses by novelty and feasibility (Ranking Agent)
5. Refine top hypotheses (Evolution Agent)
6. Connect to existing vault knowledge (Proximity Agent)
7. Synthesize final recommendations (Meta-review Agent)
8. Save to appropriate Obsidian location
```

---

## Avantajlar

1. **Sistematik yaklaşım**: Adım adım metodoloji
2. **Vault entegrasyonu**: Mevcut bilgiyle bağlantı
3. **İteratif iyileştirme**: Çoklu döngüler
4. **Dokümantasyon**: Her adım Obsidian'da kayıtlı

---

## Sınırlamalar

- Google'ınki kadar otomatik değil (manuel agent switching)
- Elo rating sistemi yok (manuel değerlendirme)
- Test-time compute scaling sınırlı (Cursor API limitleri)

---

*Bağlantılar: [[Research Project - Ana Sayfa]] | [[20260101120400-cursor-ai-not-alma]] | [[PKM MOC]]*

