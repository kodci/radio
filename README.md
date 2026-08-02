# Frekans — İnternet Radyo İstasyonu 📻

**Frekans**, modern ve şık arayüzü ile canlı internet radyo yayınlarını dinlemenizi, kendi radyo listenizi oluşturmanızı ve GitHub üzerindeki açık kaynak JSON radyo listelerini projeye aktarmanızı sağlayan responsive (mobil uyumlu) bir web uygulamasıdır.

---

## 🌟 Öne Çıkan Özellikler

- **🎛️ Sabit Alt Radyo Çalar (Fixed Bottom Player)**:
  - Ekranın en altına sabitlenmiş cam efektli (glassmorphism) alt çalar çubuğu.
  - Analog radyo kadranı (tuning dial) ve yayında jitter animasyonu.
  - Çalınan yayın için dinamik ekolayzır (equalizer bounce) görselleştirmesi.
  - Ses seviyesi (volume) kontrolü, duraklatma ve durdurma işlevleri.

- **🔲 Izgara (Grid) & Liste (List) Görünümü**:
  - İstasyonları modern kartlar (Grid) veya kompakt satırlar (Liste) halinde görüntüleme.
  - Seçilen görünüm tercihinin `localStorage` ile hatırlanması.

- **🖐️ Sürükle & Bırak Sıralama (Drag & Drop)**:
  - İstasyon sırasını kolayca sürükleyip bırakarak özelleştirme.
  - Yapılan yeni sıralamanın hafızada tutulması.

- **⚙️ Yönetim ve Ayarlar Menüsü**:
  - **Manuel İstasyon Ekleme**: İstasyon adı, akış URL'si, tür, ülke ve logo bağlantısı girerek özel yayın ekleme.
  - **GitHub'dan İçe Aktarma (JSON)**: `raw.githubusercontent.com` bağlantısı yapıştırarak açık kaynak radyo listelerini otomatik tanıma ve seçerek ekleme.
  - **Liste Temizleme & Silme**: İstasyonları tek tek veya topluca temizleme.

- **⭐ Favoriler & Arama**:
  - İstasyonları favorilere ekleme ve favorilere göre filtreleme.
  - İsim, tür ve ülkeye göre anlık canlı arama çubuğu.

- **📱 %100 Mobil Uyumluluk**:
  - Masaüstü, tablet ve mobil cihazlar için optimize edilmiş esnek (responsive) tasarım.

---

## 🛠️ Kullanılan Teknolojiler

- **HTML5**: Semantik yapılar ve modern multimedya ses oynatıcı entegrasyonu.
- **CSS3**:
  - Özel renk paleti ve tasarım değişkenleri (CSS Custom Properties).
  - Flexbox & CSS Grid dinamik düzenleri.
  - Glassmorphism (Bulanık arka plan efekti) ve CSS animasyonları.
- **Vanilla JavaScript (ES6+)**:
  - Audio API entegrasyonu ve durum yönetimi (State Management).
  - HTML5 Drag and Drop API.
  - LocalStorage ile veri kalıcılığı (Persist State).
  - Asenkron JSON Veri Getirme (Fetch API).

---

## 🚀 Çalıştırma

Proje herhangi bir derleme aşaması gerektirmeyen saf (vanilla) web teknolojileriyle geliştirilmiştir.

1. Depoyu bilgisayarınıza indirin veya klonlayın.
2. `index.html` dosyasını tarayıcınızda (Chrome, Firefox, Edge, Safari vb.) açın.

VEYA yerel bir geliştirme sunucusu ile çalıştırmak isterseniz:

```bash
# VS Code Live Server extension veya npx servor / npx http-server ile:
npx http-server .
```

---

## 📋 Örnek JSON İçe Aktarma Biçimi

GitHub'dan içe aktarma alanında kullanılacak JSON dosyası aşağıdaki gibi esnek alan adlarını destekler:

```json
[
  {
    "name": "Radyo Eksen",
    "url": "https://listen.radioking.com/radio/eksen/stream/live",
    "genre": "Alternatif Rock",
    "country": "Türkiye",
    "favicon": "https://example.com/logo.png"
  }
]
```

---

## 📄 Lisans

Bu proje MIT lisansı altında sunulmaktadır.
