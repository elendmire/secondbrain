# Deployment Rehberi

## GitHub Repository Oluşturma

1. GitHub'da yeni bir repository oluşturun:
   - Repository adı: `secondbrain` (veya istediğiniz bir isim)
   - Public veya Private seçebilirsiniz
   - README, .gitignore veya license eklemeyin (zaten var)

2. Local repository'yi GitHub'a bağlayın:

```bash
git remote add origin https://github.com/KULLANICI_ADI/secondbrain.git
git branch -M main
git push -u origin main
```

## Vercel Deploy

1. [Vercel](https://vercel.com) hesabı oluşturun (GitHub ile giriş yapabilirsiniz)

2. "New Project" butonuna tıklayın

3. GitHub repository'nizi seçin

4. Vercel otomatik olarak ayarları algılayacak:
   - **Framework Preset**: Other
   - **Build Command**: `npm run build`
   - **Output Directory**: `build`
   - **Install Command**: `npm install`

5. "Deploy" butonuna tıklayın

6. Deploy tamamlandıktan sonra, site URL'inizi alacaksınız (örn: `secondbrain.vercel.app`)

7. `quartz.config.ts` dosyasındaki `baseUrl` değerini güncelleyin:
   ```typescript
   baseUrl: "secondbrain.vercel.app", // Vercel'den aldığınız URL
   ```

8. Değişiklikleri commit edip push edin:
   ```bash
   git add quartz.config.ts
   git commit -m "Update baseUrl for Vercel"
   git push
   ```

## Otomatik Deploy

Vercel, GitHub repository'nize her push yaptığınızda otomatik olarak yeni bir deploy oluşturur.

## Custom Domain (Opsiyonel)

1. Vercel dashboard'da projenize gidin
2. "Settings" > "Domains" bölümüne gidin
3. Domain'inizi ekleyin ve DNS ayarlarını yapın
4. `quartz.config.ts` dosyasındaki `baseUrl` değerini güncelleyin

