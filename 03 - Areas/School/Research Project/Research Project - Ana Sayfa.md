---
created: 2026-01-01
modified: 2026-01-01
tags: [proje, arastirma, tubitak, wrf, ruzgar, enerji, hard-cutoff]
type: project
status: active
deadline: 
---

# 🔬 Research Project - TÜBİTAK 2209-A

> **Analysis of Extreme Wind Events Using WRF and Their Impacts on Energy Infrastructure**
> 
> *Ekstrem Rüzgar Olaylarının WRF ile Analizi ve Enerji Altyapısına Etkileri*

## 📋 Proje Özeti

Bu araştırma projesi, WRF (Weather Research and Forecasting) modeli kullanarak ekstrem rüzgar olaylarını analiz etmeyi ve bu olayların rüzgar enerji santralleri (RES) üzerindeki etkilerini incelemeyi amaçlamaktadır.

### Hard Cut-off Nedir?

Rüzgar türbinleri belirli bir rüzgar hızı aralığında çalışacak şekilde tasarlanmıştır:
- **Cut-in hızı:** ~3-4 m/s (türbin çalışmaya başlar)
- **Nominal hız:** ~12-15 m/s (maksimum verim)
- **Cut-out hızı:** ~23-25 m/s (türbin durur)

Rüzgar hızı **cut-out** hızını aştığında, türbin mekanik hasardan korunmak için otomatik olarak durur.

### Tespit Kriterleri

| Kriter | Eşik Değer | Açıklama |
|--------|------------|----------|
| **Önceki Üretim** | > 50 MW | Santral yüksek kapasitede çalışıyor olmalı |
| **Sonraki Üretim** | < 10 MW | Neredeyse tamamen durmuş olmalı |
| **Düşüş Oranı** | > %80 | Ani ve keskin bir düşüş |

---

## 📊 Genel İstatistikler (Ekim 2024 - Nisan 2025)

| Metrik | Değer |
|--------|-------|
| **Toplam Hard Cut-off Olayı** | 78 |
| **Etkilenen RES Sayısı** | 30 |
| **Toplam Üretim Kaybı** | 4,931 MW |
| **Ortalama Kayıp/Olay** | 63.2 MW |
| **Maksimum Tekil Kayıp** | 121 MW (Kangal RES) |
| **Tamamen Durma (→0 MW)** | 42 olay (%54) |

### Aylık Dağılım

| Ay | Cut-off Sayısı | Toplam Kayıp (MW) | Max Kayıp (MW) |
|----|----------------|-------------------|----------------|
| Ekim 2024 | 8 | 495 | 89 |
| Kasım 2024 | 9 | 470 | 72 |
| Aralık 2024 | 15 | 970 | 121 |
| Ocak 2025 | 7 | 433 | 77 |
| Şubat 2025 | 1 | 47 | 47 |
| **Mart 2025** | **26** | **1,856** | **109** |
| Nisan 2025 | 12 | 661 | 74 |

---

## 🎯 Proje Hedefleri

- [x] EPİAŞ verilerinden hard cut-off tespiti
- [x] 15 case study belirleme
- [ ] WRF model parametrelerinin optimizasyonu
- [ ] Case study simülasyonlarının tamamlanması
- [ ] Veri analizi ve sonuçların raporlanması
- [ ] Final rapor hazırlama

---

## 📊 15 Case Studies

Türkiye'deki RES lokasyonlarında tespit edilen en büyük 15 hard cut-off olayı:

| Case | Santral | İl | Tarih | Kayıp MW | Koordinat |
|------|---------|-----|-------|----------|-----------|
| [[Case 01 - Kangal RES]] | KANGAL RES | Sivas | 2024-12-14 00:00 | **121** | 39.15°N, 37.35°E |
| [[Case 02 - Gülpınar RES]] | GÜLPINAR RES | Çanakkale | 2025-03-27 08:00 | 109 | 39.48°N, 26.08°E |
| [[Case 03 - İstanbul RES]] | İSTANBUL RES | İstanbul | 2025-03-16 11:00 | 109 | 41.18°N, 28.35°E |
| [[Case 04 - Tatlıpınar RES]] | TATLIPINAR RES | Balıkesir | 2025-03-16 10:00 | 104 | 39.75°N, 28.15°E |
| [[Case 05 - Gülpınar RES 2]] | GÜLPINAR RES | Çanakkale | 2025-03-16 10:00 | 98 | 39.48°N, 26.08°E |
| [[Case 06 - Kangal RES 2]] | KANGAL RES | Sivas | 2024-10-18 04:00 | 89 | 39.15°N, 37.35°E |
| [[Case 07 - Evrencik RES]] | EVRENCİK RES | Kırklareli | 2025-03-16 22:00 | 89 | 41.55°N, 27.45°E |
| [[Case 08 - Üçpınar RES]] | ÜÇPINAR RES | Balıkesir | 2025-03-16 11:00 | 87 | 39.68°N, 28.10°E |
| [[Case 09 - Evrencik RES 2]] | EVRENCİK RES | Kırklareli | 2025-03-16 10:00 | 81 | 41.55°N, 27.45°E |
| [[Case 10 - Bağlar RES]] | BAĞLAR RES | Manisa | 2024-12-21 23:00 | 79 | 38.92°N, 27.58°E |
| [[Case 11 - Taşpınar RES]] | TAŞPINAR RES | İstanbul | 2025-03-16 11:00 | 77 | 41.12°N, 28.42°E |
| [[Case 12 - Saros RES]] | SAROS RES | Çanakkale | 2025-01-28 14:00 | 77 | 40.35°N, 26.55°E |
| [[Case 13 - Göktepe RES]] | GÖKTEPE RES | Yalova | 2025-03-16 11:00 | 76 | 40.55°N, 29.25°E |
| [[Case 14 - Zonguldak RES]] | ZONGULDAK RES | Sakarya | 2025-03-16 11:00 | 74 | 40.72°N, 30.18°E |
| [[Case 15 - Bozüyük RES]] | BOZÜYÜK RES | Bilecik | 2025-04-10 20:00 | 74 | 39.92°N, 30.05°E |

---

## 🌪️ 16 Mart 2025 Fırtınası - Önemli Olay

**Tek günde 15 cut-off ile rekor!** Toplam 1,098 MW kayıp.

| Saat | Santral | Üretim Değişimi | Kayıp |
|------|---------|-----------------|-------|
| 10:00 | GÜLPINAR RES | 98 → 0 MW | 98 MW |
| 10:00 | EVRENCİK RES | 81 → 0 MW | 81 MW |
| 10:00 | TATLIPINAR RES | 111 → 7 MW | 104 MW |
| 11:00 | İSTANBUL RES | 109 → 0 MW | 109 MW |
| 11:00 | ÜÇPINAR RES | 87 → 0 MW | 87 MW |
| 11:00 | TAŞPINAR RES | 77 → 0 MW | 77 MW |
| 11:00 | GÖKTEPE RES | 76 → 0 MW | 76 MW |
| 11:00 | ZONGULDAK RES | 74 → 1 MW | 73 MW |

---

## 🛠️ Metodoloji

### WRF Model Konfigürasyonu

[[WRF Simülasyon Parametreleri]] dosyasında detaylar mevcut.

- **Simülasyon Süresi:** 48 saat (12h spin-up + 24h olay öncesi + 12h olay sonrası)
- **Domain Yapısı:** D01=27km, D02=9km, D03=3km nested
- **Boundary Conditions:** ERA5 veya GFS 6-saatlik

### Veri Kaynakları

- **EPİAŞ Şeffaflık Platformu:** https://seffaflik.epias.com.tr/
- **Meteoroloji İstasyonları:** [[MTO İstasyonları]]
- **ERA5 Reanaliz Verileri**

---

## 📚 Referans Makaleler

- [[Paper - Forecasting Wind Speed Events]] - WRF-ANN hibrit model
- [[Paper - WRF Model Performance]] - WRF performans değerlendirmesi

---

## 📁 Proje Dosyaları

| Dosya | Açıklama | Konum |
|-------|----------|-------|
| Hard Cut-off Raporu | Detaylı analiz raporu | `/epias_wind_cutoff/HARD_CUTOFF_RAPOR.md` |
| Case Verileri | 15 case CSV dosyaları | `/epias_wind_cutoff/cases/` |
| Analiz Grafikleri | Görselleştirmeler | `/epias_wind_cutoff/data/` |
| Python Scriptleri | Veri çekme ve analiz | `/epias_wind_cutoff/*.py` |

---

## 🔗 İlgili Notlar

- [[School MOC]] - Akademik çalışmalar
- [[Thesis - Ana Sayfa]] - Tez çalışması (ilişkili)
- [[20260101150000-wrf-model-nedir]] - WRF Model açıklaması
- [[20260101150100-hard-cutoff-nedir]] - Hard Cut-off kavramı
- [[Programlama MOC]] - Python, veri analizi

---

## 📅 Zaman Çizelgesi

| Aşama | Durum |
|-------|-------|
| Literatür Taraması | ✅ Tamamlandı |
| EPİAŞ Veri Analizi | ✅ Tamamlandı (78 olay tespit) |
| Case Study Belirleme | ✅ Tamamlandı (15 case) |
| WRF Simülasyonları | 🔄 Devam Ediyor |
| Rapor Yazımı | ⏳ Bekliyor |

---

**Hazırlayan:** Faruk Avcı  
**İletişim:** avcio20@itu.edu.tr

*Son güncelleme: 2026-01-01*
