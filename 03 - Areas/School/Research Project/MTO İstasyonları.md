---
created: 2026-01-01
modified: 2026-01-01
tags: [meteoroloji, istasyon, veri, dogrulama, dmi]
type: reference
source: MTO_ISTASYONLARI.csv
---

# 🌡️ Meteoroloji İstasyonları - RES Eşleşmesi

> *WRF simülasyonlarının doğrulanmasında kullanılan DMİ meteoroloji istasyonları*

**Kaynak:** https://teknolojikkazalar.org/list/weather_station  
**Organizasyon:** DMİ (Devlet Meteoroloji İşleri)

## 📋 Tip Kodları

| Kod | Açıklama |
|-----|----------|
| B | Bölge İstasyonu |
| S | Sinoptik İstasyon |
| M | Meydan İstasyonu |
| T2 | Otomatik İstasyon |

---

## 📊 İstasyon - RES Eşleşme Tablosu

### Sivas Bölgesi (KANGAL RES)

| İstasyon No | İstasyon Adı | Kod | Koordinat | Tip | Yakınlık |
|-------------|--------------|-----|-----------|-----|----------|
| 17090 | Sivas Bölge | SIVS | 39°45'N, 37°01'E | B, S | 1 |
| 17874 | Kangal | KNGL | 39°14'N, 37°23'E | B | 2 |
| 17802 | Şarkışla | SRKS | 39°21'N, 36°24'E | B | 3 |

### Çanakkale Bölgesi (GÜLPINAR, SAROS RES)

| İstasyon No | İstasyon Adı | Kod | Koordinat | Tip | Yakınlık |
|-------------|--------------|-----|-----------|-----|----------|
| 17112 | Çanakkale | CNKL | 40°08'N, 26°24'E | B, S | 1 |
| 17110 | Gökçeada | GKCD | 40°12'N, 25°54'E | B, S | 2 |
| 17111 | Bozcaada | BZCD | 39°50'N, 26°04'E | B | 3 |

### İstanbul Bölgesi (İSTANBUL, TAŞPINAR RES)

| İstasyon No | İstasyon Adı | Kod | Koordinat | Tip | Yakınlık |
|-------------|--------------|-----|-----------|-----|----------|
| 17059 | Çatalca | CTLC | 41°09'N, 28°28'E | B | 1 |
| 17637 | Silivri | SLVR | 41°05'N, 28°15'E | B | 2 |
| 17636 | Florya Meydan | LTFJ | 40°59'N, 28°47'E | M, S | 3 |

### Balıkesir Bölgesi (TATLIPINAR, ÜÇPINAR RES)

| İstasyon No | İstasyon Adı | Kod | Koordinat | Tip | Yakınlık |
|-------------|--------------|-----|-----------|-----|----------|
| 17152 | Balıkesir Bölge | BLKS | 39°39'N, 27°52'E | B, S | 1 |
| 17114 | Bandırma | BAND | 40°19'N, 27°59'E | B, T2 | 2 |
| 17145 | Edremit | EDRM | 39°36'N, 27°01'E | B, S, T2 | 3 |

### Kırklareli Bölgesi (EVRENCİK RES)

| İstasyon No | İstasyon Adı | Kod | Koordinat | Tip | Yakınlık |
|-------------|--------------|-----|-----------|-----|----------|
| 17052 | Kırklareli | KRKL | 41°44'N, 27°13'E | B, S | 1 |
| 17632 | Lüleburgaz | LULB | 41°24'N, 27°21'E | B | 2 |
| 17050 | Edirne | EDRN | 41°40'N, 26°33'E | B, S | 3 |

### Manisa Bölgesi (BAĞLAR RES)

| İstasyon No | İstasyon Adı | Kod | Koordinat | Tip | Yakınlık |
|-------------|--------------|-----|-----------|-----|----------|
| 17186 | Manisa | MNIS | 38°37'N, 27°26'E | B, S | 1 |
| 17184 | Akhisar | AKHS | 38°55'N, 27°50'E | B | 2 |
| 17792 | Salihli | SLHL | 38°29'N, 28°08'E | B | 3 |

### Yalova Bölgesi (GÖKTEPE RES)

| İstasyon No | İstasyon Adı | Kod | Koordinat | Tip | Yakınlık |
|-------------|--------------|-----|-----------|-----|----------|
| 17119 | Yalova | YALV | 40°40'N, 29°17'E | B | 1 |
| 17116 | Bursa Bölge | BURS | 40°14'N, 29°01'E | B, S | 2 |
| 17066 | Kocaeli | KCAL | 40°46'N, 29°55'E | B, S | 3 |

### Sakarya Bölgesi (ZONGULDAK RES)

| İstasyon No | İstasyon Adı | Kod | Koordinat | Tip | Yakınlık |
|-------------|--------------|-----|-----------|-----|----------|
| 17069 | Adapazarı | ADPZ | 40°45'N, 30°24'E | B, S | 1 |
| 17692 | Geyve | GEYV | 40°31'N, 30°18'E | B | 2 |
| 17066 | Kocaeli | KCAL | 40°46'N, 29°55'E | B, S | 3 |

### Bilecik Bölgesi (BOZÜYÜK RES)

| İstasyon No | İstasyon Adı | Kod | Koordinat | Tip | Yakınlık |
|-------------|--------------|-----|-----------|-----|----------|
| 17702 | Bozüyük | BOZY | 39°55'N, 30°02'E | B, T2 | 1 |
| 17120 | Bilecik | BILC | 40°09'N, 29°59'E | B, S, T2 | 2 |
| 17124 | Eskişehir Meydan | LTBY | 39°47'N, 30°35'E | M, S | 3 |

---

## 📊 Veri Türleri

WRF doğrulaması için kullanılacak parametreler:

- **Rüzgar hızı** (10m, m/s)
- **Rüzgar yönü** (derece)
- **Sıcaklık** (2m, °C)
- **Basınç** (hPa)
- **Bağıl nem** (%)

---

## 📁 Kaynak Dosya

- **CSV:** `/Users/farukavci/epias_wind_cutoff/cases/MTO_ISTASYONLARI.csv`

---

## 🔗 İlgili Notlar

- [[Research Project - Ana Sayfa]] - Ana proje
- [[WRF Simülasyon Parametreleri]] - Model parametreleri
- [[Cases Özet]] - Case listesi

---

*Son güncelleme: 2026-01-01*
