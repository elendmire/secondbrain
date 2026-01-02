---
created: 2026-01-01
modified: 2026-01-01
tags: [case, ozet, wrf, analiz, hard-cutoff]
type: summary
source: 00_OZET.csv
---

# 📊 Case Studies - Özet

> *15 Hard Cut-off Case'in detaylı özet tablosu*

## 📋 Tüm Case'ler

| Case | Santral | İl | Tarih | Saat | Önceki MW | Sonraki MW | Kayıp MW | Kurulu Güç | Türbin |
|------|---------|-----|-------|------|-----------|------------|----------|------------|--------|
| CASE_01 | **KANGAL RES** | Sivas | 2024-12-14 | 00:00 | 121 | 0 | **121** | 128 MW (151.4) | 63 |
| CASE_02 | GÜLPINAR RES | Çanakkale | 2025-03-27 | 08:00 | 118 | 9 | 109 | 149 MW (165.56) | 45 |
| CASE_03 | İSTANBUL RES | İstanbul | 2025-03-16 | 11:00 | 109 | 0 | 109 | 200 MW (283.7) | 85 |
| CASE_04 | TATLIPINAR RES | Balıkesir | 2025-03-16 | 10:00 | 111 | 7 | 104 | 127 MW (131.8) | 36 |
| CASE_05 | GÜLPINAR RES | Çanakkale | 2025-03-16 | 10:00 | 98 | 0 | 98 | 149 MW (165.56) | 45 |
| CASE_06 | KANGAL RES | Sivas | 2024-10-18 | 04:00 | 89 | 0 | 89 | 128 MW (151.4) | 63 |
| CASE_07 | EVRENCİK RES | Kırklareli | 2025-03-16 | 22:00 | 97 | 9 | 89 | 130 MW (170.4) | 52 |
| CASE_08 | ÜÇPINAR RES | Balıkesir | 2025-03-16 | 11:00 | 87 | 0 | 87 | 93 MW | 31 |
| CASE_09 | EVRENCİK RES | Kırklareli | 2025-03-16 | 10:00 | 81 | 0 | 81 | 130 MW (170.4) | 52 |
| CASE_10 | BAĞLAR RES | Manisa | 2024-12-21 | 23:00 | 83 | 3 | 79 | 72 MW | 24 |
| CASE_11 | TAŞPINAR RES | İstanbul | 2025-03-16 | 11:00 | 77 | 0 | 77 | 56 MW (68) | 17 |
| CASE_12 | SAROS RES | Çanakkale | 2025-01-28 | 14:00 | 77 | 0 | 77 | 138 MW (143.5) | 41 |
| CASE_13 | GÖKTEPE RES | Yalova | 2025-03-16 | 11:00 | 76 | 0 | 76 | 118 MW | 35 |
| CASE_14 | ZONGULDAK RES | Sakarya | 2025-03-16 | 11:00 | 74 | 1 | 74 | 120 MW | 36 |
| CASE_15 | BOZÜYÜK RES | Bilecik | 2025-04-10 | 20:00 | 74 | 0 | 74 | 54 MW | 18 |

---

## 📊 İstatistikler

### Genel

| Metrik | Değer |
|--------|-------|
| Toplam Case | 15 |
| Toplam Kayıp | 1,334 MW |
| Ortalama Kayıp | 89 MW |
| Maksimum Kayıp | 121 MW (Kangal) |
| Minimum Kayıp | 74 MW |

### Tamamen Durma Oranı

- **Tamamen durma (→0 MW):** 11 case (%73)
- **Kısmi durma:** 4 case (%27)

### Bölgesel Dağılım

| Bölge | Case Sayısı |
|-------|-------------|
| Marmara (İstanbul, Balıkesir, Kırklareli) | 7 |
| Ege (Çanakkale, Manisa) | 4 |
| İç Anadolu (Sivas, Bilecik) | 3 |
| Karadeniz (Sakarya, Yalova) | 2 |

### 16 Mart 2025 Fırtınası

Bu tek günde **9 case** gerçekleşti (Case 03-09, 11, 13-14):
- Toplam kayıp: 873 MW
- Sabah 10-11 saatlerinde yoğunlaşma

---

## 📁 Kaynak Dosyalar

| Dosya | Konum |
|-------|-------|
| Özet CSV | `/epias_wind_cutoff/cases/00_OZET.csv` |
| Case CSV'leri | `/epias_wind_cutoff/cases/CASE_XX_*.csv` |

---

## 🔗 İlgili Notlar

- [[Research Project - Ana Sayfa]] - Ana proje
- [[WRF Simülasyon Parametreleri]] - Ortak parametreler
- [[MTO İstasyonları]] - Doğrulama istasyonları
- [[Case 01 - Kangal RES]] - En büyük kayıp

---

*Son güncelleme: 2026-01-01*
