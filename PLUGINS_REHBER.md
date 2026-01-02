---
created: 2026-01-01
tags: [rehber, kurulum]
type: guide
---

# 🔌 Obsidian Eklenti Kurulum Rehberi

Bu rehber, Second Brain vault'unuz için önerilen eklentileri ve kurulum adımlarını içerir.

## Ön Hazırlık

1. Obsidian'ı aç
2. Settings (⚙️) > Community Plugins
3. "Turn on community plugins" butonuna tıkla
4. "Browse" butonuyla eklenti mağazasını aç

---

## 📦 Zorunlu Eklentiler

### 1. Templater
**Amaç**: Gelişmiş şablon sistemi

**Kurulum**:
1. Browse > "Templater" ara > Install > Enable
2. Settings > Templater
3. Template folder location: `08 - Templates`
4. Trigger Templater on new file creation: ON

**Hotkey**: `Alt + N` ile yeni not oluştur

---

### 2. Dataview
**Amaç**: Notları sorgulanabilir veritabanı gibi kullanma

**Kurulum**:
1. Browse > "Dataview" ara > Install > Enable
2. Settings > Dataview
3. Enable JavaScript Queries: ON
4. Enable Inline Queries: ON

**Kullanım**: MOC notlarında otomatik listeler gösterir

---

### 3. Calendar
**Amaç**: Günlük notlar için takvim görünümü

**Kurulum**:
1. Browse > "Calendar" ara > Install > Enable
2. Sağ sidebar'da takvim görünür
3. Tarihe tıklayarak günlük not oluştur

---

### 4. Periodic Notes
**Amaç**: Günlük/Haftalık/Aylık notlar

**Kurulum**:
1. Browse > "Periodic Notes" ara > Install > Enable
2. Settings > Periodic Notes
3. Daily Notes:
   - Format: `YYYY-MM-DD`
   - Folder: `01 - Daily`
   - Template: `08 - Templates/Daily Note`

---

### 5. QuickAdd
**Amaç**: Hızlı not yakalama ve makrolar

**Kurulum**:
1. Browse > "QuickAdd" ara > Install > Enable
2. Settings > QuickAdd
3. "Add Choice" > Template
4. Name: "Yeni Zettel"
5. Template Path: `08 - Templates/Zettelkasten Note`
6. File Name Format: `{{DATE:YYYYMMDDHHmmss}}-{{NAME}}`
7. Create in folder: `06 - Zettelkasten`

**Hotkey**: `Ctrl/Cmd + Shift + N`

---

## 🤖 AI ve Akıllı Özellikler

### 6. Smart Connections
**Amaç**: AI tabanlı benzer not önerileri

**Kurulum**:
1. Browse > "Smart Connections" ara > Install > Enable
2. API key gerektirir (OpenAI veya local model)
3. İlk kurulumda tüm notları indexler

---

### 7. Copilot
**Amaç**: Vault içinde AI chat

**Kurulum**:
1. Browse > "Copilot" ara > Install > Enable
2. Settings > Copilot > API Key ekle
3. Sağ sidebar'da chat paneli açılır

---

### 8. Various Complements
**Amaç**: Otomatik tamamlama ve öneri

**Kurulum**:
1. Browse > "Various Complements" ara > Install > Enable
2. Yazarken otomatik öneri gösterir
3. Internal link önerileri aktif

---

## 📁 Organizasyon

### 9. Tag Wrangler
**Amaç**: Etiket yönetimi ve toplu düzenleme

**Kurulum**:
1. Browse > "Tag Wrangler" ara > Install > Enable
2. Tag pane'de sağ tık ile rename/merge

---

### 10. Omnisearch
**Amaç**: Gelişmiş full-text arama

**Kurulum**:
1. Browse > "Omnisearch" ara > Install > Enable
2. `Ctrl/Cmd + Shift + O` ile aç
3. Daha akıllı arama sonuçları

---

## 🎨 Verimlilik

### 11. Tasks
**Amaç**: Gelişmiş görev yönetimi

**Kurulum**:
1. Browse > "Tasks" ara > Install > Enable
2. Due date, priority, recurrence desteği
3. Global task queries

---

### 12. Kanban
**Amaç**: Proje takibi için Kanban panoları

**Kurulum**:
1. Browse > "Kanban" ara > Install > Enable
2. Yeni not oluştur > Kanban board

---

### 13. Excalidraw
**Amaç**: Görsel düşünme ve diyagramlar

**Kurulum**:
1. Browse > "Excalidraw" ara > Install > Enable
2. Yeni Excalidraw notu oluştur
3. Notlara görsel ekle

---

### 14. Advanced Tables
**Amaç**: Kolay tablo düzenleme

**Kurulum**:
1. Browse > "Advanced Tables" ara > Install > Enable
2. Tab tuşu ile hücreler arası geçiş
3. Otomatik formatlama

---

## ⌨️ Önerilen Hotkey'ler

| Eylem           | Hotkey                 |     |
| --------------- | ---------------------- | --- |
| Günlük not      | `Ctrl/Cmd + D`         |     |
| Yeni Zettel     | `Ctrl/Cmd + Shift + N` |     |
| Quick Switcher  | `Ctrl/Cmd + O`         |     |
| Command Palette | `Ctrl/Cmd + P`         |     |
| Graph View      | `Ctrl/Cmd + G`         |     |
| Omnisearch      | `Ctrl/Cmd + Shift + O` |     |

---

## 📱 iOS Kurulumu (iCloud)

1. App Store'dan Obsidian'ı indir
2. "Open folder as vault" seç
3. "iCloud Drive" > "SecondBrain" seç
4. Aynı eklentiler otomatik sync olur

---

*Kurulum sonrası bu dosyayı Archives'a taşıyabilirsiniz.*

