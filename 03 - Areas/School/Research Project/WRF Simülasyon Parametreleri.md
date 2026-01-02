---
created: 2026-01-01
modified: 2026-01-01
tags: [wrf, simulasyon, parametre, teknik]
type: reference
source: WRF_SIMULASYON_PARAMETRELERI.csv
---

# ⚙️ WRF Simülasyon Parametreleri

> *15 Hard Cut-off Case için WRF Model Konfigürasyonları*

## 📋 Genel Ayarlar

| Parametre | Değer |
|-----------|-------|
| **Optimal Simülasyon Süresi** | 48 saat |
| **Spin-up** | 12 saat |
| **Olay Öncesi** | 24 saat |
| **Olay Sonrası** | 12 saat |
| **Boundary Conditions** | ERA5 veya GFS 6-saatlik |

---

## 🗺️ Domain Yapısı (Nested)

| Domain | Çözünürlük | Kullanım |
|--------|------------|----------|
| **D01** | 27 km | Ana domain, sinoptik ölçek |
| **D02** | 9 km | Ara domain, mezo-ölçek |
| **D03** | 3 km | İç domain, yerel ölçek (RES bölgesi) |

---

## 📊 Case Bazlı Simülasyon Parametreleri

| Case | Santral | İl | Koordinat | Olay Tarihi | Kayıp MW |
|------|---------|-----|-----------|-------------|----------|
| CASE_01 | KANGAL RES | Sivas | 39.15°N, 37.35°E | 2024-12-14 00:00 | 120.7 |
| CASE_02 | GÜLPINAR RES | Çanakkale | 39.48°N, 26.08°E | 2025-03-27 08:00 | 109.1 |
| CASE_03 | İSTANBUL RES | İstanbul | 41.18°N, 28.35°E | 2025-03-16 11:00 | 108.8 |
| CASE_04 | TATLIPINAR RES | Balıkesir | 39.75°N, 28.15°E | 2025-03-16 10:00 | 104.2 |
| CASE_05 | GÜLPINAR RES | Çanakkale | 39.48°N, 26.08°E | 2025-03-16 10:00 | 97.7 |
| CASE_06 | KANGAL RES | Sivas | 39.15°N, 37.35°E | 2024-10-18 04:00 | 89.4 |
| CASE_07 | EVRENCİK RES | Kırklareli | 41.55°N, 27.45°E | 2025-03-16 22:00 | 88.6 |
| CASE_08 | ÜÇPINAR RES | Balıkesir | 39.68°N, 28.10°E | 2025-03-16 11:00 | 87.0 |
| CASE_09 | EVRENCİK RES | Kırklareli | 41.55°N, 27.45°E | 2025-03-16 10:00 | 80.9 |
| CASE_10 | BAĞLAR RES | Manisa | 38.92°N, 27.58°E | 2024-12-21 23:00 | 79.5 |
| CASE_11 | TAŞPINAR RES | İstanbul | 41.12°N, 28.42°E | 2025-03-16 11:00 | 77.2 |
| CASE_12 | SAROS RES | Çanakkale | 40.35°N, 26.55°E | 2025-01-28 14:00 | 77.1 |
| CASE_13 | GÖKTEPE RES | Yalova | 40.55°N, 29.25°E | 2025-03-16 11:00 | 76.0 |
| CASE_14 | ZONGULDAK RES | Sakarya | 40.72°N, 30.18°E | 2025-03-16 11:00 | 73.9 |
| CASE_15 | BOZÜYÜK RES | Bilecik | 39.92°N, 30.05°E | 2025-04-10 20:00 | 73.6 |

---

## ⏰ Simülasyon Zaman Pencereleri

Her case için WRF simülasyon zamanları:

| Case | WRF Start | WRF End | Analysis Start | Analysis End |
|------|-----------|---------|----------------|--------------|
| CASE_01 | 2024-12-12 12:00 | 2024-12-14 12:00 | 2024-12-13 00:00 | 2024-12-14 12:00 |
| CASE_02 | 2025-03-25 20:00 | 2025-03-27 20:00 | 2025-03-26 08:00 | 2025-03-27 20:00 |
| CASE_03 | 2025-03-14 23:00 | 2025-03-16 23:00 | 2025-03-15 11:00 | 2025-03-16 23:00 |
| CASE_04 | 2025-03-14 22:00 | 2025-03-16 22:00 | 2025-03-15 10:00 | 2025-03-16 22:00 |
| CASE_05 | 2025-03-14 22:00 | 2025-03-16 22:00 | 2025-03-15 10:00 | 2025-03-16 22:00 |
| CASE_06 | 2024-10-16 16:00 | 2024-10-18 16:00 | 2024-10-17 04:00 | 2024-10-18 16:00 |
| CASE_07 | 2025-03-15 10:00 | 2025-03-17 10:00 | 2025-03-15 22:00 | 2025-03-17 10:00 |
| CASE_08 | 2025-03-14 23:00 | 2025-03-16 23:00 | 2025-03-15 11:00 | 2025-03-16 23:00 |
| CASE_09 | 2025-03-14 22:00 | 2025-03-16 22:00 | 2025-03-15 10:00 | 2025-03-16 22:00 |
| CASE_10 | 2024-12-20 11:00 | 2024-12-22 11:00 | 2024-12-20 23:00 | 2024-12-22 11:00 |
| CASE_11 | 2025-03-14 23:00 | 2025-03-16 23:00 | 2025-03-15 11:00 | 2025-03-16 23:00 |
| CASE_12 | 2025-01-27 02:00 | 2025-01-29 02:00 | 2025-01-27 14:00 | 2025-01-29 02:00 |
| CASE_13 | 2025-03-14 23:00 | 2025-03-16 23:00 | 2025-03-15 11:00 | 2025-03-16 23:00 |
| CASE_14 | 2025-03-14 23:00 | 2025-03-16 23:00 | 2025-03-15 11:00 | 2025-03-16 23:00 |
| CASE_15 | 2025-04-09 08:00 | 2025-04-11 08:00 | 2025-04-09 20:00 | 2025-04-11 08:00 |

---

## 🔬 Önerilen Fizik Parametrizasyonları

| Şema Tipi | Önerilen | Alternatif |
|-----------|----------|------------|
| Mikrofizik | Thompson | Morrison |
| Kümülüs | Kain-Fritsch | Grell-3D |
| PBL | YSU | MYNN |
| Yüzey Tabakası | MM5 Similarity | Revised MM5 |
| Arazi Yüzeyi | Noah | Noah-MP |
| Radyasyon (SW) | RRTMG | Dudhia |
| Radyasyon (LW) | RRTMG | RRTM |

---

## 📁 Kaynak Dosya

- **CSV:** `/Users/farukavci/epias_wind_cutoff/cases/WRF_SIMULASYON_PARAMETRELERI.csv`

---

## 🔗 İlgili Notlar

- [[Research Project - Ana Sayfa]] - Ana proje
- [[MTO İstasyonları]] - Doğrulama verileri
- [[20260101150000-wrf-model-nedir]] - WRF Model açıklaması
- [[Cases Özet]] - Case listesi

---

*Son güncelleme: 2026-01-01*
