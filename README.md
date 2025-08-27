# News Site

Statik HTML/CSS ile hazırlanmış, duyarlı (responsive) bir haber sitesi arayüzü.

## İçerik ve Sayfalar

- `index.html`: Ana sayfa. Manşet bölümünde öne çıkan haber ve "Latest News" grid yapısında kartlar.
- `article.html`: Tekil haber detay sayfası. Yan tarafta abonelik çağrısı ve kategori listesi.
- `about.html`: Hakkında sayfası iskeleti.

Not: Navigasyondaki `blog.html` ve `contact.html` linkleri şu an için sayfalar oluşturulmadığından 404 verecektir.

## Özellikler

- Duyarlı tasarım: `css/mobile.css` ile 768px ve 600px kırılımlarında düzenler.
- Grid yerleşimi: Kart listeleri ve layout CSS Grid ile kuruldu.
- Yardımcı sınıflar: `btn`, `card`, `bg-*`, `py-*`, `mb-*` gibi utility sınıfları ile hızlı stil.
- Varlıklar: Görseller `img/` altında, başlık ve gövde yazıları Google Fonts ile.
- Sosyal ikonlar: Font Awesome 5 kullanımı.

## Teknolojiler

- Saf HTML5 ve CSS3
- Google Fonts (`Lato`, `Varela Round`)
- Font Awesome (CDN)

## Proje Yapısı

```
News-Site/
  ├─ index.html
  ├─ about.html
  ├─ article.html
  ├─ css/
  │  ├─ style.css
  │  └─ mobile.css
  └─ img/
     ├─ logo.png
     ├─ rowing.jpeg
     ├─ img-1.webp
     ├─ img-2.webp
     └─ img-3.webp
```

## Çalıştırma

Statik bir projedir; bir HTTP sunucusu ile yerelde açabilirsiniz.

- Tarayıcıda doğrudan `index.html` dosyasını açın veya
- VS Code Live Server ile kök dizinde "Open with Live Server" deyin veya
- Python ile geçici sunucu başlatın:

```bash
cd /Users/ahseneminyorulmaz/Documents/News-Site
python3 -m http.server 5500
# Ardından tarayıcıda: http://localhost:5500
```

## Düzenleme İpuçları

- Renk paleti ve boyutlar `css/style.css` içindeki `:root` CSS değişkenlerinden yönetilir.
- Manşet görseli `css/style.css` → `#header::before` içinde `img/rowing.jpeg` olarak tanımlıdır.
- Kart yapısı ve sayfa gridleri `#main-articles .articles-container` ve `.page-container` sınıflarıyla kontrol edilir.
- Mobil kırılımlar `css/mobile.css` dosyasındadır.

## Erişilebilirlik ve UX Notları

- Link metinlerini ve `alt` niteliklerini anlamlı içerikle güncellemeniz önerilir.
- Form (footer abonelik) örnektir; gerçek entegrasyon yoktur.

## Yol Haritası / Geliştirme Önerileri

- `blog.html` ve `contact.html` sayfalarını ekleyin ya da menüden kaldırın.
- Aktif menü durumu için sayfa bazlı `active` sınıfını güncelleyin.
- Basit bir derleme/varlık optimizasyonu (minify, görsel sıkıştırma) ekleyin.
- Basit bir JS ile mobil menü (hamburger) ve form doğrulama eklenebilir.

## Lisans

Bu proje eğitim ve demo amaçlıdır. İhtiyaçlarınıza göre bir lisans dosyası (`LICENSE`) ekleyebilirsiniz.


