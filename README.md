# Frekans — İnternet Radyo İstasyonu 📻

**Frekans**, modern ve şık arayüzü ile canlı internet radyo yayınlarını dinlemenizi, radyo istasyonlarınızı düzenlemenizi, listenizi JSON olarak dışarı aktarmanızı ve GitHub üzerindeki açık kaynak radyo listelerini projeye aktarmanızı sağlayan responsive (mobil uyumlu) bir web uygulamasıdır.

---

## 🌟 Öne Çıkan Özellikler

- **🎛️ Sabit Alt Radyo Çalar (Fixed Bottom Player)**:
  - Ekranın en altına sabitlenmiş cam efektli (glassmorphism) alt çalar çubuğu.
  - Analog radyo kadranı (tuning dial) ve yayında jitter animasyonu.
  - Çalınan yayın için dinamik ekolayzır (equalizer bounce) görselleştirmesi.
  - Ses seviyesi (volume) kontrolü, duraklatma ve durdurma işlevleri.

- **✏️ İstasyon Düzenleme & Düzenleme Modu**:
  - **Düzenleme Modu Toggle**: Ayarlar menüsünden istenildiği zaman açılıp kapatılabilen düzenleme modu.
  - **İstasyon Güncelleme**: İstasyon adı, yayın akış URL'si, müzik türü, ülke ve logo bilgilerini kolayca düzenleme imkanı.
  - Düzenlenen yayının anında çalara ve hafızaya yansıması.

- **💾 Listeyi Dışarı Aktarma (JSON Export)**:
  - Ayarlar menüsünden tek tıkla mevcut tüm radyo listenizi JSON formatında bilgisayarınıza indirme.
  - İndirilen veriler ile radyo listenizi yedekleyebilir veya başka cihazlara aktarabilirsiniz.

- **🚨 Modern Özel Silme Onayı Modal Dialog**:
  - Tarayıcının varsayılan pop-up'ları yerine uygulamanın koyu temasına ve cam efektine tam uyumlu özel onay penceresi.
  - Yanlışlıkla radyo silmeyi önleyen güvenli onay akışı.

- **🖐️ Görsel Tutamaçlı Sürükle & Bırak Sıralama (Drag & Drop)**:
  - Kartların sağ üst köşesinde yer alan 6 noktalı özel tutamaç (`DRAG_ICON`) ile istasyon sırasını kolayca değiştirme.
  - Yapılan yeni sıralamanın `localStorage` üzerinde saklanması.

- **🔲 Izgara (Grid) & Liste (List) Görünümü**:
  - İstasyonları modern kartlar (Grid) veya kompakt satırlar (Liste) halinde görüntüleme.
  - Hızlı kart içi `Oynat/Duraklat` butonları ve canlı yayın rozetleri (`YAYINDA` / `SEÇİLDİ` / `CANLI`).
  - Seçilen görünüm tercihinin hafızada tutulması.

- **⚙️ Gelişmiş Yönetim Menüsü**:
  - **Manuel İstasyon Ekleme**: Form aracılığıyla özel yayın ekleme.
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

## 📋 Örnek JSON İçe & Dışarı Aktarma Biçimi

Projeden dışarı aktarılan ve içe aktarmada desteklenen JSON formatı:

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
