---
created: 2026-01-01 16:37
modified: 2026-01-01 16:37
tags: [protokol, deneysel, compound-events, epidemiyoloji]
type: experimental-protocol
related: [20260101161700-hipotez-compound-events-saglik]
status: draft
---

# Deneysel Protokol: Compound Climate Events ve Sağlık Etkileşimleri

> **Hipotez:** [[20260101161700-hipotez-compound-events-saglik]]  
> **Araştırma Sorusu:** Eşzamanlı iklim tehlikeleri (sıcak hava dalgası + hava kirliliği) sağlık üzerinde nasıl etkileşim göstermektedir?

---

## 1. Araştırma Tasarımı

### 1.1 Çalışma Tipi
**Epidemiyolojik Analiz: Case-Crossover + Time-Series**

- **Tasarım 1:** Case-crossover (bireysel düzey)
- **Tasarım 2:** Time-series (popülasyon düzeyi)
- **Tasarım 3:** Mekanizma çalışması (klinik)

### 1.2 Çalışma Süresi
- **Veri toplama:** 5-10 yıl geriye dönük + 2 yıl ileriye dönük
- **Analiz:** 6 ay
- **TOPLAM:** 2.5-3 yıl

---

## 2. Çalışma Bölgesi ve Veri Kaynakları

### 2.1 Çalışma Bölgesi

**Kriterler:**
- Nüfus: >500,000
- Sıcak hava dalgası riski yüksek
- Hava kirliliği sorunu var
- Veri erişimi: Sağlık ve çevre verileri mevcut

**Önerilen Şehirler:**
- İstanbul, Türkiye
- Los Angeles, ABD
- Delhi, Hindistan
- Mexico City, Meksika
- Beijing, Çin

### 2.2 Veri Kaynakları

#### Meteoroloji Verileri
- **Kaynak:** Meteoroloji istasyonları, ERA5 reanaliz
- **Parametreler:**
  - Günlük maksimum/minimum sıcaklık
  - Rüzgar hızı ve yönü
  - Nem oranı
  - Basınç
- **Çözünürlük:** Günlük, saatlik (opsiyonel)

#### Hava Kalitesi Verileri
- **Kaynak:** Hava kalitesi izleme istasyonları
- **Parametreler:**
  - PM2.5, PM10 (μg/m³)
  - O₃ (ppb)
  - NO₂ (ppb)
  - SO₂ (ppb)
- **Çözünürlük:** Günlük ortalama, saatlik maksimum

#### Sağlık Verileri
- **Kaynak:** Sağlık bakanlığı, hastaneler
- **Parametreler:**
  - Günlük ölüm sayıları (tüm nedenler, spesifik nedenler)
  - Acil servis başvuruları
  - Hastane yatışları
  - ICD-10 kodları

---

## 3. Compound Events Tanımlama

### 3.1 Tanım Kriterleri

**Compound Event Tipi 1: Sıcak Hava Dalgası + Yüksek Ozon**
- Sıcak hava dalgası: Maksimum sıcaklık >35°C (veya şehre özgü eşik)
- Yüksek ozon: O₃ >100 ppb (veya şehre özgü eşik)
- Düşük rüzgar: Rüzgar hızı <2 m/s (opsiyonel)

**Compound Event Tipi 2: Sıcak Hava Dalgası + Yüksek PM2.5**
- Sıcak hava dalgası: >35°C
- Yüksek PM2.5: PM2.5 >50 μg/m³
- Düşük rüzgar: <2 m/s

**Compound Event Tipi 3: Sıcak Hava Dalgası + Yüksek Ozon + Yüksek PM2.5**
- Üçlü kombinasyon

### 3.2 Eşik Değerleri

**Şehre Özgü Eşikler:**
- Her şehir için kendi eşikleri belirlenmeli
- Yöntem: 90. veya 95. persentil
- Alternatif: Mutlak değerler (WHO standartları)

---

## 4. Analiz Planı

### 4.1 Tasarım 1: Case-Crossover Analizi

**Amaç:** Bireysel düzeyde compound events'in etkisini ölçmek

**Tasarım:**
- **Case günleri:** Compound event günleri
- **Control günleri:** Aynı hafta, aynı gün (ör: aynı gün, farklı hafta)
- **Matching:** Hafta içi/hafta sonu, mevsim

**Model:**
```
logit(P[Event]) = α + β₁(Compound_t) + β₂(Heat_t) + β₃(Ozone_t) + 
                  β₄(Heat_t × Ozone_t) + γControls_t
```

**Beklenen Sonuç:**
- β₄ > 0: Etkileşim (sinergistik etki)
- β₄ = β₂ + β₃: Toplamsal etki
- β₄ > β₂ + β₃: Sinergistik etki

### 4.2 Tasarım 2: Time-Series Analizi

**Amaç:** Popülasyon düzeyinde etkiyi ölçmek

**Model:**
```
Y_t = α + β₁(Heat_t) + β₂(Ozone_t) + β₃(PM25_t) + 
      β₄(Heat_t × Ozone_t) + β₅(Heat_t × PM25_t) + 
      β₆(Ozone_t × PM25_t) + β₇(Heat_t × Ozone_t × PM25_t) +
      γTrend_t + δSeason_t + ε_t
```

**Açıklamalar:**
- Y_t: Günlük ölüm/hastane başvurusu sayısı
- Heat_t: Sıcak hava dalgası göstergesi (0/1)
- Ozone_t: Yüksek ozon göstergesi (0/1)
- PM25_t: Yüksek PM2.5 göstergesi (0/1)
- Trend: Zaman trendi
- Season: Mevsimsel düzeltme

**Analiz Yöntemi:**
- Distributed lag models (DLM)
- Lag 0-7 gün
- Non-linear sıcaklık etkisi (spline)

### 4.3 Tasarım 3: Mekanizma Çalışması

**Amaç:** Fizyolojik mekanizmaları anlamak

**Katılımcılar:**
- 50-100 sağlıklı yetişkin
- 20-30 KOAH hastası
- 20-30 astım hastası

**Ölçümler:**
- **Solunum fonksiyon testleri:**
  - FEV1, FVC (spirometri)
  - Peak flow
- **İnflamasyon belirteçleri:**
  - IL-6, TNF-α (kan örneği)
  - FeNO (nefes testi)
- **Oksidatif stres:**
  - 8-iso-PGF2α (idrar)

**Tasarım:**
- Compound event günlerinde ölçüm
- Kontrol günlerinde ölçüm
- Karşılaştırma

---

## 5. Veri Toplama

### 5.1 Geriye Dönük Veri Toplama

**Süre:** 5-10 yıl geriye dönük

**Veriler:**
- Meteoroloji: Günlük veriler
- Hava kalitesi: Günlük veriler
- Sağlık: Günlük ölüm/hastane verileri

**Kaynaklar:**
- Resmi kurumlar (meteoroloji, çevre, sağlık)
- Açık veri platformları
- Araştırma kurumları

### 5.2 İleriye Dönük Veri Toplama

**Süre:** 2 yıl

**Amaç:** Geriye dönük analizi doğrulamak

**Veriler:**
- Aynı parametreler
- Ek: Bireysel düzey veriler (opsiyonel)

---

## 6. Analiz Detayları

### 6.1 Birincil Analiz: Etkileşim Testi

**Hipotez:**
- H₀: β₄ = 0 (etkileşim yok, toplamsal)
- H₁: β₄ > 0 (sinergistik etki)

**Test:**
- Likelihood ratio test
- AIC/BIC karşılaştırması

### 6.2 İkincil Analizler

#### A. Eşik Analizi
- Farklı eşik değerleri test et
- Optimal eşik belirleme
- ROC analizi

#### B. Lag Analizi
- Hangi lag'de en güçlü etki?
- Distributed lag models
- Lag 0-7 gün

#### C. Alt Grup Analizleri
- Yaş gruplarına göre
- Cinsiyete göre
- Kronik hastalık durumuna göre
- Sosyoekonomik duruma göre

#### D. Coğrafi Analiz
- Şehir içi farklılıklar
- Isı adası etkisi
- Hava kirliliği dağılımı

### 6.3 Hassasiyet Analizleri

1. **Farklı eşik değerleri**
2. **Farklı lag yapıları**
3. **Farklı kontrol değişkenleri**
4. **Farklı zaman pencereleri**

---

## 7. Erken Uyarı Sistemi Geliştirme

### 7.1 Compound Events Erken Uyarı Modeli

**Girdiler:**
- Meteoroloji tahminleri (1-3 gün öncesi)
- Hava kalitesi tahminleri
- Mevsimsel faktörler

**Çıktılar:**
- Compound event olasılığı
- Beklenen sağlık etkisi
- Önerilen müdahaleler

**Model Tipi:**
- Machine learning (Random Forest, XGBoost)
- Veya: İstatistiksel model (logistic regression)

### 7.2 Etkinlik Değerlendirmesi

**Tasarım:** Quasi-experimental
- Erken uyarı sistemi uygulanan şehirler
- Kontrol şehirler

**Ölçüm:**
- Erken uyarı sonrası sağlık sonuçları
- Müdahale oranları
- Ölüm/hastane başvurusu azalması

---

## 8. Etik Hususlar

### 8.1 Veri Gizliliği
- Anonimleştirme
- Toplu veri kullanımı (bireysel değil)
- GDPR/KVKK uyumu

### 8.2 Etik Onay
- Üniversite etik kurulu (mekanizma çalışması için)
- Veri kullanım izinleri
- Şehir yönetimi izinleri

---

## 9. Zaman Çizelgesi

| Faz | Süre | Aktivite |
|-----|------|----------|
| **Faz 1: Veri Toplama** | Ay 1-12 | Geriye dönük veri toplama ve temizleme |
| **Faz 2: Analiz** | Ay 13-18 | Epidemiyolojik analiz |
| **Faz 3: Mekanizma** | Ay 19-24 | Klinik çalışma (opsiyonel) |
| **Faz 4: Erken Uyarı** | Ay 25-30 | Model geliştirme ve test |
| **Faz 5: Doğrulama** | Ay 31-36 | İleriye dönük veri toplama |

---

## 10. Bütçe Tahmini

| Kalem | Miktar | Birim Fiyat | Toplam |
|-------|--------|-------------|--------|
| Personel | 3 yıl | $50,000/yıl | $150,000 |
| Veri satın alma/lisans | - | - | $20,000 |
| Mekanizma çalışması | - | - | $80,000 |
| Erken uyarı sistemi geliştirme | - | - | $40,000 |
| Analiz yazılımları | - | - | $10,000 |
| **TOPLAM** | - | - | **$300,000** |

---

## 11. Olası Sınırlamalar ve Çözümler

### Sınırlama 1: Veri Kalitesi
**Sorun:** Eksik veriler, hatalı kayıtlar  
**Çözüm:** Veri temizleme, imputation, hassasiyet analizi

### Sınırlama 2: Confounding
**Sorun:** Diğer faktörler sonuçları etkileyebilir  
**Çözüm:** Kontrol değişkenleri, zaman trend analizi

### Sınırlama 3: Genellenebilirlik
**Sorun:** Şehir özelinde sonuçlar  
**Çözüm:** Çoklu şehir analizi, meta-analiz

---

## 12. Beklenen Çıktılar

### Bilimsel Çıktılar
- 2-3 hakemli makale
- Compound events tanımları
- Etkileşim mekanizmaları

### Pratik Çıktılar
- Erken uyarı sistemi
- Politika önerileri
- Halk sağlığı rehberleri

---

## 🔗 İlgili Notlar

- [[20260101161700-hipotez-compound-events-saglik]] - Ana hipotez
- [[Literatur Taramasi - Hipotez 3 - Compound Events]] - Literatür taraması
- [[Urban Health Climate Change - Araştırma Planı]] - Ana plan

---

*Durum: 📝 Protokol taslağı hazır*  
*Son güncelleme: 2026-01-01 16:37*

