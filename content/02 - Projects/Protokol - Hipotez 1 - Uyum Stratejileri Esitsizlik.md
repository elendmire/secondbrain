---
created: 2026-01-01 16:35
modified: 2026-01-01 16:35
tags: [protokol, deneysel, uyum, esitsizlik, rct]
type: experimental-protocol
related: [20260101161500-hipotez-uyum-stratejileri-esitsizlik]
status: draft
---

# Deneysel Protokol: Eşitlik Odaklı Uyum Stratejilerinin Sağlık Eşitsizliği Üzerindeki Etkisi

> **Hipotez:** [[20260101161500-hipotez-uyum-stratejileri-esitsizlik]]  
> **Araştırma Sorusu:** Eşitlik odaklı uyum stratejileri, geleneksel yaklaşımlara göre savunmasız gruplarda daha fazla sağlık iyileşmesi sağlar mı?

---

## 1. Araştırma Tasarımı

### 1.1 Çalışma Tipi
**Quasi-Experimental Design: Difference-in-Differences (DID)**

- **Grup 1:** Eşitlik odaklı uyum stratejileri uygulanan mahalleler (Müdahale)
- **Grup 2:** Geleneksel uyum stratejileri uygulanan mahalleler (Kontrol 1)
- **Grup 3:** Uyum stratejisi olmayan mahalleler (Kontrol 2)

### 1.2 Çalışma Süresi
- **Hazırlık:** 6 ay
- **Müdahale öncesi veri toplama:** 12 ay (baseline)
- **Müdahale uygulama:** 18 ay
- **Müdahale sonrası takip:** 12 ay
- **TOPLAM:** 4 yıl

---

## 2. Çalışma Bölgesi ve Örneklem

### 2.1 Çalışma Bölgesi Seçimi

**Kriterler:**
- Nüfus: 500,000-2,000,000 arası şehirler
- İklim: Sıcak hava dalgası riski yüksek
- Sosyoekonomik çeşitlilik: Farklı gelir seviyelerinde mahalleler
- Veri erişimi: Sağlık ve çevre verileri mevcut

**Önerilen Şehirler:**
- İstanbul, Türkiye
- Barcelona, İspanya
- Melbourne, Avustralya
- Los Angeles, ABD

### 2.2 Mahalle Seçimi

**Her şehirde:**
- 6 mahalle (2 müdahale, 2 geleneksel, 2 kontrol)
- Toplam: 24 mahalle (4 şehir × 6 mahalle)

**Eşleştirme Kriterleri:**
- Benzer nüfus yoğunluğu
- Benzer sosyoekonomik profil (başlangıçta)
- Benzer iklim riski
- Benzer altyapı durumu

### 2.3 Örneklem Büyüklüğü

**Güç Analizi:**
- Hedef etki büyüklüğü: d = 0.5 (orta etki)
- Güç: 80%
- Anlamlılık: α = 0.05
- **Gerekli örneklem:** ~200 kişi/mahalle
- **Toplam:** ~4,800 katılımcı (24 mahalle × 200)

**Katılımcı Seçimi:**
- Rastgele hane seçimi (random sampling)
- Yaş: 18+ (özellikle 65+ yaşlılar)
- Yerleşik: En az 1 yıldır mahallede yaşıyor
- Onay: Bilgilendirilmiş onam

---

## 3. Müdahale Detayları

### 3.1 Eşitlik Odaklı Uyum Stratejileri (Müdahale Grubu)

#### A. Yeşil Alan Dağılımı
- **Hedef:** Her mahallede eşit yeşil alan erişimi
- **Metrik:** 500m yarıçap içinde park/yeşil alan
- **Uygulama:**
  - Düşük gelirli mahallelerde yeni parklar
  - Mevcut parkları iyileştirme
  - Sokak ağaçlandırması
  - Topluluk bahçeleri

#### B. Soğuk Yüzeyler
- **Hedef:** Tüm mahallelerde eşit dağılım
- **Uygulama:**
  - Yansıtıcı çatılar (düşük gelirli konutlarda)
  - Soğuk kaldırımlar
  - Gölgelendirme yapıları
  - Yeşil çatılar (topluluk merkezlerinde)

#### C. Erken Uyarı Sistemleri
- **Hedef:** Erişilebilir ve çok dilli
- **Uygulama:**
  - SMS, telefon, radyo uyarıları
  - Topluluk merkezlerinde görsel uyarılar
  - Çok dilli materyaller
  - Savunmasız gruplara özel iletişim

### 3.2 Geleneksel Uyum Stratejileri (Kontrol 1)

- Mevcut şehir planlama yaklaşımı
- Merkezi bölgelerde yoğunlaşmış uygulamalar
- Standart erken uyarı sistemleri

### 3.3 Kontrol Grubu (Kontrol 2)

- Müdahale yok
- Sadece gözlem

---

## 4. Veri Toplama

### 4.1 Sağlık Sonuçları (Bağımlı Değişkenler)

#### Birincil Sonuçlar
1. **Sıcaklık kaynaklı ölümler**
   - Kaynak: Ölüm kayıtları
   - ICD-10 kodları: X30 (aşırı sıcaklık), I00-I99 (kardiyovasküler)
   - Ölçüm: Aylık/yıllık oranlar

2. **Acil servis başvuruları**
   - Kaynak: Hastane kayıtları
   - Kategoriler: Sıcak çarpması, dehidrasyon, solunum sorunları
   - Ölçüm: Günlük başvuru sayıları

3. **Hastane yatışları**
   - Kaynak: Hastane veritabanları
   - Süre: Yatış süresi, yoğun bakım ihtiyacı
   - Ölçüm: Aylık yatış oranları

#### İkincil Sonuçlar
4. **Sağlık eşitliği metrikleri**
   - Gini katsayısı (sağlık sonuçları için)
   - Eşitlik indeksleri (Theil, Atkinson)
   - Ölçüm: Yıllık değişim

5. **Yaşam kalitesi**
   - Anket: SF-36 veya EQ-5D
   - Ölçüm: 6 ayda bir

### 4.2 Bağımsız Değişkenler

#### Müdahale Değişkenleri
- Müdahale tipi (eşitlik odaklı vs. geleneksel)
- Müdahale yoğunluğu (yeşil alan m²/kişi)
- Müdahale süresi

#### Çevresel Değişkenler
- **Sıcaklık:**
  - Günlük maksimum/minimum sıcaklık
  - Gece sıcaklığı
  - Isı adası yoğunluğu (UHI index)
  - Kaynak: Meteoroloji istasyonları, uydu verileri

- **Hava Kalitesi:**
  - PM2.5, PM10
  - O₃, NO₂
  - Kaynak: Hava kalitesi izleme istasyonları

- **Yeşil Alan Erişimi:**
  - Park alanı/kişi
  - Yeşil alan erişilebilirliği (500m yarıçap)
  - NDVI (Normalized Difference Vegetation Index)
  - Kaynak: Uydu görüntüleri, GIS analizi

#### Sosyoekonomik Değişkenler
- Gelir seviyesi (hane bazlı)
- Eğitim düzeyi
- Konut kalitesi
- Klima erişimi
- Kaynak: Anket, nüfus sayımı verileri

#### Kontrol Değişkenleri
- Yaş, cinsiyet
- Kronik hastalık varlığı
- İlaç kullanımı
- Sosyal destek

### 4.3 Veri Toplama Araçları

#### Anketler
- **Demografik anket:** Yaş, cinsiyet, gelir, eğitim
- **Sağlık anketi:** Kronik hastalıklar, ilaç kullanımı
- **Yaşam kalitesi:** SF-36 veya EQ-5D
- **Erişim anketi:** Yeşil alan, sağlık hizmetleri erişimi

#### Fiziksel Ölçümler
- **Sıcaklık sensörleri:** İç mekan ve dış mekan
- **Hava kalitesi monitörleri:** PM2.5, O₃
- **Uydu görüntüleri:** NDVI, yüzey sıcaklığı

#### Sağlık Verileri
- Ölüm kayıtları (resmi kayıtlar)
- Hastane veritabanları
- Acil servis kayıtları

---

## 5. Analiz Planı

### 5.1 Birincil Analiz: Difference-in-Differences (DID)

**Model:**
```
Y_it = α + β₁(Treatment_i × Post_t) + β₂Treatment_i + β₃Post_t + 
       γX_it + δZ_i + ε_it
```

**Açıklamalar:**
- Y_it: Sağlık sonucu (mahalle i, zaman t)
- Treatment_i: Müdahale grubu (1) vs. kontrol (0)
- Post_t: Müdahale sonrası dönem (1) vs. öncesi (0)
- X_it: Zaman değişken çevresel faktörler
- Z_i: Zaman değişmeyen mahalle özellikleri

**Beklenen Sonuç:**
- β₁ > 0: Müdahale grubunda müdahale sonrası daha fazla iyileşme

### 5.2 İkincil Analizler

#### A. Eşitlik Metrikleri Analizi
- Gini katsayısı hesaplama (sağlık sonuçları için)
- Eşitlik indeksleri (Theil, Atkinson)
- Zaman içinde değişim analizi

#### B. Alt Grup Analizleri
- Gelir seviyesine göre
- Yaş gruplarına göre (65+, 18-64, <18)
- Kronik hastalık durumuna göre

#### C. Mekanizma Analizi
- Yeşil alan erişimi → sıcaklık azalması → sağlık iyileşmesi
- Mediation analizi (Baron & Kenny yöntemi)

### 5.3 Hassasiyet Analizleri

1. **Farklı eşik değerleri:** Müdahale yoğunluğu
2. **Farklı zaman pencereleri:** 6 ay, 12 ay, 18 ay
3. **Farklı kontrol grupları:** Sadece geleneksel vs. hiç müdahale yok
4. **Missing data:** Multiple imputation

---

## 6. Etik Hususlar

### 6.1 Etik Onay
- Üniversite etik kurulu onayı
- Şehir yönetimi izinleri
- Katılımcı bilgilendirilmiş onamı

### 6.2 Etik Sorunlar ve Çözümler

**Sorun 1: Kontrol Grubuna Müdahale Yapılmaması**
- **Çözüm:** Çalışma sonrası kontrol grubuna da müdahale
- **Açıklama:** "Delayed intervention" yaklaşımı

**Sorun 2: Veri Gizliliği**
- **Çözüm:** Anonimleştirme, veri şifreleme
- **GDPR/KVKK uyumu**

**Sorun 3: Topluluk Beklentileri**
- **Çözüm:** Açık iletişim, gerçekçi beklenti yönetimi
- **Topluluk danışma kurulu**

---

## 7. Zaman Çizelgesi

| Faz | Süre | Aktivite |
|-----|------|----------|
| **Faz 0: Hazırlık** | Ay 1-6 | Etik onay, şehir seçimi, mahalle eşleştirme |
| **Faz 1: Baseline** | Ay 7-18 | Veri toplama (müdahale öncesi) |
| **Faz 2: Müdahale** | Ay 19-36 | Müdahale uygulama |
| **Faz 3: Takip** | Ay 37-48 | Veri toplama (müdahale sonrası) |
| **Faz 4: Analiz** | Ay 49-54 | Veri analizi, rapor yazımı |

---

## 8. Bütçe Tahmini

| Kalem | Miktar | Birim Fiyat | Toplam |
|-------|--------|-------------|--------|
| Personel (araştırmacılar) | 4 yıl | $50,000/yıl | $200,000 |
| Veri toplama (anketörler) | 2 yıl | $30,000/yıl | $60,000 |
| Ekipman (sensörler, monitörler) | - | - | $40,000 |
| Müdahale maliyetleri | - | - | $150,000 |
| Veri analizi yazılımları | - | - | $10,000 |
| Seyahat ve konaklama | - | - | $30,000 |
| **TOPLAM** | - | - | **$490,000** |

---

## 9. Olası Sınırlamalar ve Çözümler

### Sınırlama 1: Kontaminasyon (Müdahale Sızıntısı)
**Sorun:** Kontrol grubundaki kişiler müdahale mahallelerine gidebilir  
**Çözüm:** Coğrafi olarak izole mahalleler seç, analizde kontrol et

### Sınırlama 2: Dış Faktörler
**Sorun:** Diğer politika değişiklikleri sonuçları etkileyebilir  
**Çözüm:** Kontrol değişkenleri, zaman trend analizi

### Sınırlama 3: Uzun Süreli Takip
**Sorun:** Katılımcı kaybı, müdahale sürdürülebilirliği  
**Çözüm:** Düzenli iletişim, teşvikler, topluluk sahiplenmesi

---

## 10. Beklenen Çıktılar

### Bilimsel Çıktılar
- 3-4 hakemli makale
- Konferans sunumları
- Metodoloji rehberi

### Pratik Çıktılar
- Şehir planlamacıları için eşitlik odaklı rehber
- Politika önerileri
- Etkinlik raporu

---

## 🔗 İlgili Notlar

- [[20260101161500-hipotez-uyum-stratejileri-esitsizlik]] - Ana hipotez
- [[Literatur Taramasi - Hipotez 1 - Uyum Stratejileri Esitsizlik]] - Literatür taraması
- [[Urban Health Climate Change - Araştırma Planı]] - Ana plan

---

*Durum: 📝 Protokol taslağı hazır*  
*Son güncelleme: 2026-01-01 16:35*

