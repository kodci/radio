# Frekans — İnternet Radyo İstasyonu 📻

**Frekans**, modern ve şık arayüzü ile canlı internet radyo yayınlarını dinlemenizi, dinamik kategori etiketlerine göre filtreleme yapmanızı, radyo listenizi düzenlemenizi ve JSON formatında dışarı/içe aktarmanızı sağlayan responsive (mobil uyumlu) gelişmiş bir web uygulamasıdır.

---

## 🌟 Öne Çıkan Özellikler

- **🎛️ Sabit Alt Radyo Çalar (Fixed Bottom Player)**:
  - Ekranın en altına sabitlenmiş cam efektli (glassmorphism) alt çalar çubuğu.
  - Radyo amblemi/logosu varsa oynatıcıda gösterim, yoksa veya seçim yapılmadığında analog kadran (`dial`) gösterimi.
  - Dinamik ekolayzır animasyonu ve parlayan canlı yayın rozetleri (`YAYINDA` / `SEÇİLDİ` / `ÇEVRİMDİŞİ / HATA`).
  - Masaüstünde hızlı ses seviyesi kaydırıcısı ve mute toggle; **Mobilde açılır şeffaf dikey ses seviyesi popover penceresi (`Volume Popover`)**.

- **🏷️ Dinamik Kategori & Etiket Filtreleme (Category Pill Filters)**:
  - Eklenen radyoların müzik türleri/etiketleri taranarak otomatik olarak üst kontrolde **Kategori Butonları** oluşturulur.
  - *Tüm Yayınlar*, *Favoriler*, *Pop*, *Rock*, *Türk Sanat Müziği*, *Haber*, *Caz* vb. kategorilere göre tek tıkla canlı süzme.
  - Mobilde ve masaüstünde taşma yapmayan kaydırılabilir (scrollable) şık kategori çubuğu.

- **✏️ Düzenleme Modu & İstasyon Güncelleme**:
  - Ayarlar menüsünden istenildiği zaman açılıp kapatılabilen **Düzenleme Modu**.
  - İstasyon adı, yayın akış URL'si, müzik türü, ülke ve logo bilgilerini manuel düzenleme.

- **💾 JSON Dışarı Aktarma & İçe Aktarma Rehberi**:
  - **Dışarı Aktar**: Tüm radyo listenizi JSON formatında tek tıkla yedekleyin veya indirin.
  - **JSON İçe Aktarma Rehberi**: Ayarlar menüsünden açılan modern modal pencerede örnek JSON format şeması.

- **🖐️ Masaüstü & Mobilde Otomatik Kaydırmalı Sürükle-Bırak (Touch Drag & Drop with Auto-Scroll)**:
  - 6 noktalı tutamaç simgesi (`drag-handle`) ile radyoların sırasını kolayca değiştirin.
  - Mobilde dokunmatik ekranlar (`touchstart`/`touchmove`) ve sayfa kenarlarında otomatik kaydırma (`auto-scroll`) desteği.

- **🚨 Modern Özel Silme Onayı Modal Dialog**:
  - Tarayıcının native `confirm()` pop-up'ı yerine koyu temalı özel onay dialog penceresi.

- **🔲 Izgara (Grid) & Liste (List) Görünümü**:
  - Radyoları modern Grid kartları veya Liste satırları halinde inceleme.
  - Kart içi anlık dinle/duraklat butonları ve sağa hizalanmış durumu rozetleri.

- **📱 %100 Mobil & Masaüstü Uyumlu Responsive Tasarım**:
  - Ekran boyutuna göre kendini ayarlayan padding ve çakışma önleyici dikey boşluklar.

---

## 🛠️ Kullanılan Teknolojiler

- **HTML5**: Semantik yapılar ve modern multimedya ses oynatıcı entegrasyonu.
- **CSS3**:
  - Özel renk paleti ve tasarım değişkenleri (CSS Custom Properties).
  - Flexbox & CSS Grid dinamik düzenleri.
  - Glassmorphism (Bulanık arka plan efekti) ve CSS animasyonları.
- **Vanilla JavaScript (ES6+)**:
  - Audio API entegrasyonu, hata/çevrimdışı akış yönetimi ve durum yönetimi.
  - Touch Events API & Drag and Drop API (Auto-scroll destekli).
  - LocalStorage ile veri kalıcılığı (Persist State).
  - Asenkron JSON Veri Getirme (Fetch API).

---

## 🚀 Çalıştırma

Proje herhangi bir derleme veya paket kurucu gerektirmeyen saf (vanilla) web teknolojileriyle geliştirilmiştir.

1. Depoyu bilgisayarınıza indirin veya klonlayın.
2. `index.html` dosyasını tarayıcınızda (Chrome, Firefox, Edge, Safari vb.) açın.

VEYA yerel bir geliştirme sunucusu ile çalıştırmak isterseniz:

```bash
# VS Code Live Server extension veya npx http-server ile:
npx http-server .
```

---

## 📋 Örnek JSON İçe & Dışarı Aktarma Formatı

```json
[
  {
    "name": "Radyo Eksen",
    "url": "https://listen.radioking.com/radio/eksen/stream/live",
    "genre": "Alternatif Rock",
    "country": "Türkiye",
    "favicon": "https://example.com/logo.png",
    "favorite": false
  }
]
```

---

## 📄 Lisans

Bu proje MIT lisansı altında sunulmaktadır.
