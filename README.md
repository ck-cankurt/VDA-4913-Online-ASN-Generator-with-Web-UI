# 📋 VDA 4913 ASN JSON Generator

[![VDA 4913](https://img.shields.io/badge/VDA-4913-blue.svg)](https://github.com/ck-cankurt/vda4913-generator)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

<div align="center">

## 🚀 Uygulamayı Açmak İçin Tıklayın

[![Open Application](https://img.shields.io/badge/🚀%20Uygulamayı%20Aç-vda4913_generator.html-brightgreen?style=for-the-badge&logo=rocket)](./vda4913_generator.html)

</div>

---

## 📖 Hakkında

**VDA 4913 ASN JSON Generator**, otomotiv endüstrisinde kullanılan VDA 4913 standardına uygun **Advanced Shipping Notice (ASN)** JSON dosyalarını kolayca oluşturmanızı sağlayan web tabanlı bir araçtır.

### ✨ Özellikler

- 🏗️ **Komple VDA 4913 Yapısı**: Tüm segmentler dahil (711, 712, 713, 714, 715, 719)
- 📦 **Paketleme Yönetimi**: Palet ve koli boyutları için ayrı alanlar
- 📏 **VDA Standartları**: Tüm formatlar VDA 4913 standardına uygun
- 💾 **JSON Export**: Tek tıkla dosya indirme
- 📋 **Kopyala**: JSON'u panoya kopyalama
- 🎨 **Modern UI**: Responsive ve kullanıcı dostu arayüz
- 📱 **Mobil Uyumlu**: Tüm cihazlarda çalışır

---

## 🏗️ VDA 4913 Segment Yapısı

### 📄 711 - Teslimat Bilgileri (preSetOfDeliveryInformation)
- Data Recipient/Sender Number
- Transmission Number Old/New
- Transmission Date

### 🚛 712 - Taşıma Detayları (transportDetails)
- Delivery Relation Number
- Carrier & Handover bilgileri
- Delivery Weight & Transport Type

### 📋 713 - İrsaliye Detayları (deliveryNoteDetails)
- Delivery Note Number & Dispatch Date
- Unloading Area & Type Of Dispatch
- Order Number & Factory/Supplier bilgileri

### 🏷️ 714 - Pozisyon Detayları (deliveryNotePositionDetails)
- Article Numbers (Customer/Supplier)
- Country Of Production
- Quantity Of Delivery (VDA formatında)
- Unit Of Measure & Position bilgileri

### 📦 715 - Paketleme Bilgileri (packageInformation)
- Palet ve koli boyutları
- VDA standartlarına uygun formatlamalar
- Filling Amount & Packaging Dimensions

### 📊 719 - Segment Özeti (segmentSummary)
- Otomatik sayaç hesaplamaları
- Her segment için doğru counter değerleri

---

## 🚀 Kullanım

### 1️⃣ Ana Parametreler
- **Palet Sayısı**: Oluşturulacak palet sayısı
- **Koli Sayısı**: Her palet için koli sayısı
- **Başlangıç Numarası**: Paketleme numarası başlangıcı

### 2️⃣ Segment Bilgileri
Her VDA segmenti için gerekli bilgileri doldurun:
- Teslimat bilgileri (711)
- Taşıma detayları (712)
- İrsaliye detayları (713)
- Pozisyon detayları (714)
- Paketleme bilgileri (715)

### 3️⃣ Boyut Girişi
- **Koli Boyutları**: Length, Width, Height (mm)
- **Palet Boyutları**: Length, Width, Height (mm)

### 4️⃣ JSON Oluşturma
- **🚀 VDA 4913 ASN JSON Oluştur** butonuna tıklayın
- JSON çıktısını görüntüleyin
- **📋 Kopyala** ile panoya kopyalayın
- **💾 JSON Kaydet** ile dosya indirin

---

## 📋 VDA 4913 Format Standartları

### 🔢 Filling Amount (715_07)
- **Format**: 13 karakter, sağa hizalı
- **Ondalık**: 3 basamak (nokta olmadan)
- **Örnek**: `120` → `0000001200000`

### 📏 Packaging Dimensions (715_10)
- **Format**: Length(4)Width(4)Height(4) mm
- **Toplam**: 12 karakter
- **Örnek**: `110011001440` (1100mm x 1100mm x 144mm)

### 📊 Quantity Of Delivery (714_06)
- **Format**: 13 karakter, sağa hizalı
- **Ondalık**: 3 basamak (nokta olmadan)
- **Örnek**: `13440` → `0000013440000`

### 🔢 Counter (719 segment)
- **Format**: 7 karakter, sağa hizalı
- **Örnek**: `1` → `0000001`

---

## 🎨 Ekran Görüntüleri

<div align="center">

### Ana Form
<img width="861" height="832" alt="image" src="https://github.com/user-attachments/assets/ebb474a4-cf7f-40f9-9d13-75bbbbe0ccd0" />


### JSON Çıktısı
<img width="807" height="712" alt="image" src="https://github.com/user-attachments/assets/a690c500-b5f0-495d-8a5b-8f1d9e99c3e6" />


### Dosya İndirme
<img width="749" height="497" alt="image" src="https://github.com/user-attachments/assets/a0902778-16b7-4fdf-8ce7-3eb1c31bf6c5" />


</div>

---

## 🛠️ Teknik Detaylar

### 📁 Dosya Yapısı
```
vda4913-generator/
├── vda4913_generator.html    # Ana uygulama dosyası
├── vda4913.json             # Örnek VDA 4913 JSON
├── README.md                # Bu dosya
└── LICENSE                  # MIT Lisansı
```

### 🔧 Teknolojiler
- **HTML5**: Modern web standartları
- **CSS3**: Responsive tasarım ve animasyonlar
- **JavaScript ES6+**: Modern JavaScript özellikleri
- **VDA 4913**: Otomotiv endüstrisi standardı

### 📱 Tarayıcı Desteği
- ✅ Chrome 60+
- ✅ Firefox 55+
- ✅ Safari 12+
- ✅ Edge 79+

---

## 📝 Örnek Kullanım

### 1. Form Doldurma
```html
<!-- Ana Parametreler -->
Palet Sayısı: 9
Koli Sayısı: 16
Başlangıç Numarası: 252610001

<!-- Segment Bilgileri -->
Data Recipient Number: ALICI NUMARASI
Data Sender Number: GONDEREN NUMARASI
Delivery Note Number: IRSALIYE NUMARASI
...
```

### 2. JSON Çıktısı
```json
{
  "_711_preSetOfDeliveryInformation": {
    "_71101_recordName": "711",
    "_71102_versionNumber": "03",
    "_71103_dataRecipientNumber": "ALICI NUMARASI",
    ...
  },
  "group1": [
    {
      "group1SequenceId": 1,
      "_712_transportDetails": {
        ...
      }
    }
  ]
}
```

### 3. Dosya İndirme
- Dosya adı: `IRSALIYE NUMARASI_vda4913.json`
- Format: UTF-8 JSON
- Boyut: ~5-10 KB (segment sayısına göre)

---

## 🤝 Katkıda Bulunma

Bu projeye katkıda bulunmak için:

1. **Fork** yapın
2. **Feature branch** oluşturun (`git checkout -b feature/AmazingFeature`)
3. **Commit** yapın (`git commit -m 'Add some AmazingFeature'`)
4. **Push** yapın (`git push origin feature/AmazingFeature`)
5. **Pull Request** açın

### 🐛 Bug Bildirimi
Bir bug bulduysanız, lütfen [Issues](https://github.com/ck-cankurt/vda4913-generator/issues) bölümünden bildirin.

### 💡 Özellik İsteği
Yeni özellik önerileriniz için [Issues](https://github.com/ck-cankurt/vda4913-generator/issues) bölümünü kullanın.

---

## 📄 Lisans

Bu proje MIT lisansı altında lisanslanmıştır. Detaylar için [LICENSE](LICENSE) dosyasına bakın.

---

## 👨‍💻 Geliştirici

**@ck-cankurt**
- GitHub: [@ck-cankurt](https://github.com/ck-cankurt)
- LinkedIn: [Profil](https://linkedin.com/in/can-kurt)

---

## 🙏 Teşekkürler

- **VDA (Verband der Automobilindustrie)** - VDA 4913 standardı için
- **Otomotiv Endüstrisi** - Standartların geliştirilmesi için
- **Açık Kaynak Topluluğu** - Sürekli destek için

---

<div align="center">

### ⭐ Bu projeyi beğendiyseniz yıldız vermeyi unutmayın!

[![GitHub stars](https://img.shields.io/github/stars/ck-cankurt/vda4913-generator?style=social)](https://github.com/ck-cankurt/vda4913-generator/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/ck-cankurt/vda4913-generator?style=social)](https://github.com/ck-cankurt/vda4913-generator/network/members)

---

**🚀 VDA 4913 ASN JSON Generator ile profesyonel teslimat bildirimlerinizi kolayca oluşturun!**

</div>

