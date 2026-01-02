# SecondBrain - Digital Garden

Bu repo, Obsidian vault'unu Quartz static site generator kullanarak web'de yayınlamak için kullanılmaktadır.

## Kurulum

```bash
npm install
```

## Yerel Geliştirme

```bash
npm run start
```

Site `http://localhost:8080` adresinde çalışacaktır.

## Build

```bash
npm run build
```

Build çıktısı `build/` klasöründe oluşturulacaktır.

## Vercel Deploy

Bu repo Vercel'de otomatik olarak deploy edilir. Her push'ta otomatik olarak yeni bir build oluşturulur.

## Yapı

- `content/` - Obsidian vault içeriği (symlink)
- `quartz/` - Quartz framework kodu
- `quartz.config.ts` - Quartz yapılandırması
- `quartz.layout.ts` - Layout yapılandırması
- `build/` - Build çıktısı (gitignore'da)

