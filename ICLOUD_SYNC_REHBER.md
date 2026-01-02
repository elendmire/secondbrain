---
created: 2026-01-01
tags: [rehber, kurulum, icloud]
type: guide
---

# ☁️ iCloud Sync Kurulum Rehberi

Bu rehber, SecondBrain vault'unuzu iCloud üzerinden tüm Apple cihazlarınızda senkronize etmenizi sağlar.

---

## 📍 Vault Konumu

```
~/Library/Mobile Documents/com~apple~CloudDocs/SecondBrain/
```

Bu konum otomatik olarak iCloud Drive ile senkronize edilir.

---

## 💻 Mac Kurulumu

Vault zaten iCloud Drive'da oluşturuldu. Obsidian'da açmak için:

1. Obsidian'ı aç
2. "Open folder as vault" seç
3. Finder'da `Cmd + Shift + G` ile git:
   ```
   ~/Library/Mobile Documents/com~apple~CloudDocs/SecondBrain
   ```
4. Klasörü seç ve aç

---

## 📱 iPhone/iPad Kurulumu

1. **App Store'dan Obsidian'ı indir**

2. **Vault'u aç**:
   - Obsidian'ı aç
   - "Create new vault" VEYA "Open folder as vault" seç
   - "Store in iCloud" seç ✓
   - "SecondBrain" klasörünü seç

3. **İlk sync'i bekle**:
   - iCloud tüm dosyaları indirmeli
   - Dosyalar yanında bulut simgesi varsa indiriliyor demektir
   - Tamamlanana kadar bekle

---

## ⚠️ Önemli Uyarılar

### Sync Çakışmaları

iCloud bazen aynı dosyanın iki versiyonunu oluşturabilir:
- `Note.md`
- `Note 2.md` veya `Note (conflict).md`

**Çözüm**:
1. Her iki dosyayı da aç
2. İçerikleri karşılaştır
3. Doğru olanı koru, diğerini sil

### .obsidian Klasörü

Eklenti ayarları `.obsidian` klasöründe saklanır. Bu klasör bazen sync sorunlarına neden olabilir.

**Eğer sorun yaşarsanız**:
1. Tüm cihazlarda Obsidian'ı kapat
2. Mac'te `.obsidian` klasörünü yedekle
3. Cihazları sırayla aç

### Büyük Dosyalar

PDF ve görseller için:
1. Dosyayı açmadan önce iCloud'un indirmesini bekle
2. Çok büyük dosyalardan kaçın (>50MB)
3. Görselleri optimize et

---

## 🔄 En İyi Pratikler

1. **Aynı anda tek cihaz**: Aynı notu iki cihazda aynı anda düzenleme
2. **Sync bekle**: Cihaz değiştirmeden önce sync'in tamamlanmasını bekle
3. **Düzenli kontrol**: Haftada bir conflict dosyalarını kontrol et
4. **Yedekleme**: Önemli notları ayrıca yedekle

---

## 🔧 Sorun Giderme

### Dosyalar görünmüyor
1. iOS Settings > Apple ID > iCloud > iCloud Drive: ON
2. Obsidian uygulamasının iCloud erişimi olduğundan emin ol
3. Cihazı yeniden başlat

### Sync yavaş
1. WiFi bağlantısını kontrol et
2. iCloud depolama alanını kontrol et
3. Büyük dosyaları temizle

### Eklentiler sync olmuyor
1. Tüm cihazlarda Obsidian'ı güncelle
2. .obsidian/plugins klasörünü kontrol et
3. Eklentileri her cihazda manuel aktifle

---

## 📊 Sync Durumu Kontrolü

Mac'te Terminal'de çalıştır:
```bash
brctl status
```

veya Finder'da iCloud Drive'a git ve dosya simgelerini kontrol et:
- ☁️ = Sadece iCloud'da
- ⬇️ = İndiriliyor
- ✓ = Yerel kopya mevcut

---

*Bu rehberi okuduktan sonra Archives'a taşıyabilirsiniz.*

