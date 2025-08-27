# 📰 News Site - Modern Haber Web Sitesi

Bu proje, modern ve responsive bir haber web sitesi arayüzü olan **News Site**'ın kaynak kodlarını içerir. Manşet görseli, kategori rozetleri ve kart tabanlı liste yapısıyla temiz, okunabilir ve mobil uyumlu bir deneyim sunar.

## 📋 İçindekiler

- [Özellikler](#özellikler)
- [Teknolojiler](#teknolojiler)
- [Kurulum](#kurulum)
- [Proje Yapısı](#proje-yapısı)
- [Sayfalar](#sayfalar)
- [Tasarım ve Responsive Detayları](#tasarım-ve-responsive-detayları)
- [Görseller](#görseller)
- [Katkıda Bulunma](#katkıda-bulunma)
- [Lisans](#lisans)

## ✨ Özellikler

- 🎨 **Modern ve Responsive Tasarım**: 768px ve 600px kırılımları için optimize edilmiş düzen
- 📰 **Ana Sayfa**: Manşet (hero) alanı ve "Latest News" kart grid’i
- 🧭 **Sabit Navigasyon**: Üst menü sticky, sosyal medya ikonları entegre
- 🏷️ **Kategori Rozetleri**: `bg-primary`, `bg-secondary` renk varyasyonları
- 🧩 **Utility Sınıfları**: `btn`, `card`, `bg-*`, `py-*`, `mb-*` ile hızlı stil
- 🧱 **CSS Grid Düzenleri**: Kart listeleri ve sayfa düzenleri grid ile kurulu
- 🖼️ **Hero Arka Planı**: `rowing.jpeg` ile blur-overlay etkili başlık alanı

## 🛠️ Teknolojiler

- **HTML5**: Semantik ve erişilebilir yapılar
- **CSS3**: CSS Grid, yardımcı sınıflar ve değişkenler (CSS Custom Properties)
- **Font Awesome 5**: Sosyal medya ikonları (CDN)
- **Google Fonts**: `Lato` ve `Varela Round`

## 🚀 Kurulum

1. Proje dizinine gidin ve yerelde başlatın:
   ```bash
   cd /Users/ahseneminyorulmaz/Documents/News-Site
   python3 -m http.server 5500
   # Tarayıcı: http://localhost:5500
   ```

2. Veya doğrudan `index.html` dosyasını tarayıcıda açabilirsiniz. Canlı yenileme için VS Code Live Server önerilir.

## 📁 Proje Yapısı

```
News-Site/
├── index.html        # Ana sayfa (manşet + kart grid)
├── article.html      # Haber detay sayfası (meta + yan sütunlar)
├── about.html        # Hakkında sayfası (iskelet)
├── css/
│   ├── style.css     # Ana stil, grid ve komponent stilleri
│   └── mobile.css    # Mobil düzen ve kırılımlar
├── img/
│   ├── logo.png
│   ├── rowing.jpeg   # Manşet arka plan görseli
│   ├── img-1.webp
│   ├── img-2.webp
│   └── img-3.webp
└── README.md
```

## 📄 Sayfalar

### 🏠 Ana Sayfa (`index.html`)
- **Hero/Manşet**: Kategori rozeti, başlık ve kısa özet; `Read More` butonu
- **Latest News**: 3 sütunlu kart grid (tablet ve mobilde 2/1 sütuna düşer)
- **Footer**: Abonelik formu, linkler ve sosyal medya alanı

### 📰 Haber Detay (`article.html`)
- **Kapak Görseli** ve **Başlık**
- **Meta Alanı**: Yazar, tarih ve kategori rozeti (`.meta`)
- **Yan Sütunlar**: `Join Us` çağrısı ve `Categories` listesi

### ℹ️ Hakkında (`about.html`)
- Gelecek içerikler için temel sayfa iskeleti

Not: Menüde görünen `blog.html` ve `contact.html` henüz ekli değil; tıklayınca 404 verebilir.

## 🎯 Tasarım ve Responsive Detayları

### 🎨 Tasarım
- **Renk Paleti**: `:root` içinde `--primary-color`, `--secondary-color`, `--dark-color`, `--light-color`
- **Tipografi**: Başlıklar `Varela Round`, gövde `Lato`
- **Bileşenler**: `btn`, `card`, `category` rozetleri, utility spacing sınıfları
- **Hero Arka Planı**: `#header::before` ile tam ekran arka plan ve opaklık efekti

### 📱 Responsive
- **Kırılımlar**: `css/mobile.css` ile 768px ve 600px altında grid yeniden akış
- **Grid Uyarlamaları**: `#main-articles .articles-container` ve `.page-container` sütun sayısı küçülür
- **Navigasyon**: Sosyal ikonlar mobilde gizlenir, menü tek sütuna iner

### ⚡ Performans
- **CDN Kullanımı**: Font Awesome ve Google Fonts hız için CDN üzerinden
- **Optimize Görseller**: `.webp` görseller tercih edilmiş

## 🖼️ Görseller

Projede kullanılan başlıca görseller:
- `img/rowing.jpeg`: Manşet arka planı
- `img/img-1.webp`, `img/img-2.webp`, `img/img-3.webp`: Haber kart görselleri
- `img/logo.png`: Logo

## 🤝 Katkıda Bulunma

1. Bu depoyu fork edin
2. Branch oluşturun (`git checkout -b feature/yeni-ozellik`)
3. Değişiklikleri commit edin (`git commit -m "Yeni özellik eklendi"`)
4. Branch’i push edin (`git push origin feature/yeni-ozellik`)
5. Pull Request açın

## 📞 İletişim

Sorularınız için:
- **E-posta**: ahseneminyorulmaz@gmail.com
- **GitHub**: github.com/ahsenemin

## 📄 Lisans

Bu proje eğitim ve demo amaçlıdır. Dilerseniz bir lisans dosyası (`LICENSE`) ekleyebilirsiniz.


