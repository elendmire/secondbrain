---
created: 2026-01-01
modified: 2026-01-01
tags: [case, wrf, kangal, res, simulasyon, sivas]
type: case-study
status: pending
date: 2024-12-14
location: Sivas
loss_mw: 121
---

# 🌬️ Case 01 - Kangal RES

> **En büyük tekil hard cut-off olayı: 121 MW kayıp**

## 📋 Case Bilgileri

| Alan | Değer |
|------|-------|
| **Case ID** | CASE_01 |
| **Santral** | KANGAL RES |
| **İl** | Sivas |
| **Koordinat** | 39.15°N, 37.35°E |
| **Olay Tarihi** | 2024-12-14 00:00 |
| **Kurulu Güç** | 128 MW (151.4 MW) |
| **Türbin Sayısı** | 63 |
| **Durum** | ⏳ WRF simülasyonu bekliyor |

---

## 📊 Üretim Verisi

| Metrik | Değer |
|--------|-------|
| **Önceki Üretim** | 121 MW |
| **Sonraki Üretim** | 0 MW |
| **Kayıp** | **121 MW** |
| **Düşüş Oranı** | %100 (tam durma) |

---

## ⏰ WRF Simülasyon Penceresi

| Parametre | Değer |
|-----------|-------|
| **WRF Start** | 2024-12-12 12:00 UTC |
| **WRF End** | 2024-12-14 12:00 UTC |
| **Analysis Start** | 2024-12-13 00:00 UTC |
| **Analysis End** | 2024-12-14 12:00 UTC |
| **Toplam Süre** | 48 saat |

---

## 🌡️ Doğrulama İstasyonları

[[MTO İstasyonları]] dosyasından Kangal RES için en yakın istasyonlar:

| Sıra | İstasyon | Kod | Koordinat |
|------|----------|-----|-----------|
| 1 | Sivas Bölge | SIVS | 39°45'N, 37°01'E |
| 2 | Kangal | KNGL | 39°14'N, 37°23'E |
| 3 | Şarkışla | SRKS | 39°21'N, 36°24'E |

---

## 🔬 Analiz Notları

- En büyük tekil kayıp olayı (121 MW)
- Gece yarısı (00:00) gerçekleşmiş
- Aynı santral CASE_06'da da etkilenmiş (89 MW, 2024-10-18)
- İç Anadolu'da izole lokasyon

---

## 📁 Dosyalar

| Dosya | Konum |
|-------|-------|
| Case CSV | `/epias_wind_cutoff/cases/CASE_01_KANGAL_RES_20241214.csv` |

---

## 🔗 İlgili Notlar

- [[Research Project - Ana Sayfa]] - Ana proje
- [[Cases Özet]] - Tüm case'ler
- [[Case 06 - Kangal RES 2]] - Aynı lokasyon, farklı tarih
- [[WRF Simülasyon Parametreleri]] - Kullanılacak parametreler
- [[MTO İstasyonları]] - Doğrulama istasyonları

---

*Case ID: 01 | Kayıp: 121 MW | Tarih: 2024-12-14*
