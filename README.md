# Hece Gayrimenkul Sapanca — Web Sitesi

Sapanca, Maşukiye ve Kırkpınar bölgesinde gayrimenkul (satılık villa, arsa, kiralık konut) danışmanlığı için çok dilli (TR / EN / AR), SEO odaklı, tek sayfalık tanıtım sitesi.

- **Alan adı:** https://sapancahecegroup.com
- **E-posta:** info@sapancahecegroup.com
- **Telefon:** +90 544 583 41 61 · +90 553 686 07 04

## Dosya Yapısı

```
.
├── index.html            # Türkçe (varsayılan)
├── en/index.html         # English
├── ar/index.html         # العربية (RTL)
├── 404.html
├── assets/
│   ├── css/style.css
│   ├── js/main.js
│   └── img/og-image.svg  # Sosyal paylaşım görseli
├── favicon.svg
├── site.webmanifest
├── sitemap.xml
├── robots.txt
├── CNAME                 # GitHub Pages özel alan adı
└── .nojekyll
```

## GitHub Pages ile Yayına Alma

1. Bu klasördeki tüm dosyaları yeni bir GitHub deposuna yükleyin (depo adı fark etmez).
2. **Settings → Pages** bölümüne gidin.
3. **Source** olarak `Deploy from a branch` seçin; branch: `main`, klasör: `/ (root)`.
4. **Custom domain** alanına `sapancahecegroup.com` yazın (CNAME dosyası zaten var).
5. Alan adı sağlayıcınızda DNS kayıtlarını ayarlayın:
   - `A` kayıtları (apex/`@`) → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - `CNAME` (`www`) → `<kullanıcıadı>.github.io`
6. Pages ayarlarında **Enforce HTTPS** seçeneğini işaretleyin.

> DNS yayılması birkaç saat sürebilir. Yayına alındıktan sonra site `https://sapancahecegroup.com` adresinden açılır.

## Yayın Sonrası SEO (önerilir)

- **Google Search Console**'a siteyi ekleyip `sitemap.xml` adresini gönderin.
- **Google İşletme Profili** (Google Business Profile) kaydını doğrulayın — "Sapanca Hece Real Estate" işletmesi haritalarda mevcut; sahipliği alıp telefon, web sitesi ve fotoğrafları ekleyin. Yerel aramada (Sapanca emlak) en çok bunu etkiler.
- Sosyal medya hesaplarını açıp her sayfadaki yapısal verideki `sameAs` alanına bağlantıları ekleyin.

## Düzenleme İpuçları

- Telefon numaraları, e-posta ve metinler her dil dosyasının içinde düz HTML olarak yer alır.
- Renk ve yazı tipi ayarları `assets/css/style.css` dosyasının en üstündeki `:root` değişkenlerindedir.
- Harita, API anahtarı gerektirmeyen Google Maps embed bağlantısıyla gömülüdür (konum: 40.6918028, 30.2002814).
