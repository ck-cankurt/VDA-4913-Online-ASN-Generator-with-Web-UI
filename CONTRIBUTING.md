# 🤝 Katkıda Bulunma Rehberi

VDA 4913 ASN JSON Generator projesine katkıda bulunmak için teşekkürler! Bu rehber, projeye nasıl katkıda bulunabileceğinizi açıklar.

## 📋 İçindekiler

- [Kod Katkısı](#kod-katkısı)
- [Bug Bildirimi](#bug-bildirimi)
- [Özellik İsteği](#özellik-isteği)
- [Dokümantasyon](#dokümantasyon)
- [Test](#test)
- [Pull Request Süreci](#pull-request-süreci)

## 🚀 Kod Katkısı

### 1. Fork ve Clone
```bash
# GitHub'da fork yapın
# Sonra local'e clone edin
git clone https://github.com/YOUR_USERNAME/vda4913-generator.git
cd vda4913-generator
```

### 2. Branch Oluşturma
```bash
# Feature branch oluşturun
git checkout -b feature/amazing-feature
# veya bug fix için
git checkout -b bugfix/fix-issue-123
```

### 3. Değişikliklerinizi Yapın
- Kodunuzu yazın
- VDA 4913 standartlarına uygun olduğundan emin olun
- Responsive tasarımı koruyun
- Modern JavaScript kullanın

### 4. Test Edin
```bash
# Tarayıcıda test edin
# Farklı tarayıcılarda çalıştığını kontrol edin
# Mobil cihazlarda test edin
```

### 5. Commit ve Push
```bash
git add .
git commit -m "feat: add amazing feature"
git push origin feature/amazing-feature
```

## 🐛 Bug Bildirimi

### Bug Bildirirken Şunları Dahil Edin:

1. **Açıklayıcı Başlık**
2. **Adım Adım Reproduksiyon**
3. **Beklenen Davranış**
4. **Gerçek Davranış**
5. **Screenshot/Video** (varsa)
6. **Tarayıcı ve İşletim Sistemi Bilgisi**

### Örnek Bug Raporu:
```markdown
**Bug Başlığı:** JSON export butonu çalışmıyor

**Açıklama:** 
JSON Kaydet butonuna tıkladığımda dosya indirilmiyor.

**Adımlar:**
1. Formu doldurun
2. "VDA 4913 ASN JSON Oluştur" butonuna tıklayın
3. "JSON Kaydet" butonuna tıklayın

**Beklenen:** Dosya indirilmeli
**Gerçek:** Hiçbir şey olmuyor

**Tarayıcı:** Chrome 120.0.6099.109
**OS:** Windows 11
```

## 💡 Özellik İsteği

### Özellik İsteğinde Şunları Dahil Edin:

1. **Özellik Açıklaması**
2. **Kullanım Senaryosu**
3. **VDA 4913 Uyumluluğu**
4. **Alternatif Çözümler**

### Örnek Özellik İsteği:
```markdown
**Özellik:** XML export desteği

**Açıklama:** 
JSON'a ek olarak XML formatında da export yapabilmek istiyorum.

**Kullanım Senaryosu:**
Bazı sistemler XML formatını tercih ediyor. Bu özellik ile daha geniş uyumluluk sağlanabilir.

**VDA Uyumluluğu:**
VDA 4913 standardı XML formatını da destekliyor.
```

## 📚 Dokümantasyon

### README.md Güncellemeleri
- Yeni özellikler için dokümantasyon ekleyin
- Screenshot'ları güncelleyin
- Kullanım örneklerini genişletin

### Kod Dokümantasyonu
```javascript
/**
 * VDA 4913 formatında filling amount formatlar
 * @param {number} value - Formatlanacak değer
 * @returns {string} VDA standartında formatlanmış string
 * @example formatFillingAmount(120) // "0000001200000"
 */
function formatFillingAmount(value) {
    // Implementation
}
```

## 🧪 Test

### Manuel Test Checklist:
- [ ] Form validasyonu çalışıyor
- [ ] JSON oluşturma doğru
- [ ] Dosya indirme çalışıyor
- [ ] Kopyala özelliği çalışıyor
- [ ] Responsive tasarım korunuyor
- [ ] VDA standartlarına uygun

### Tarayıcı Testleri:
- [ ] Chrome (son 2 versiyon)
- [ ] Firefox (son 2 versiyon)
- [ ] Safari (son 2 versiyon)
- [ ] Edge (son 2 versiyon)

## 🔄 Pull Request Süreci

### PR Açmadan Önce:
1. **Branch'inizi güncelleyin:**
   ```bash
   git checkout main
   git pull origin main
   git checkout feature/amazing-feature
   git rebase main
   ```

2. **Kodunuzu kontrol edin:**
   - Kod temiz ve okunabilir
   - Gereksiz kod yok
   - VDA standartlarına uygun
   - Responsive tasarım korunmuş

### PR Açarken:
1. **Açıklayıcı başlık yazın**
2. **Değişiklikleri detaylandırın**
3. **Screenshot ekleyin** (UI değişiklikleri için)
4. **Test sonuçlarını belirtin**
5. **İlgili issue'ları linkleyin**

### PR Template:
```markdown
## 📝 Değişiklik Açıklaması
Bu PR ne yapıyor?

## 🔗 İlgili Issue
Fixes #123

## 🧪 Test
- [ ] Manuel test yapıldı
- [ ] Farklı tarayıcılarda test edildi
- [ ] Responsive tasarım kontrol edildi

## 📸 Screenshot
(UI değişiklikleri için)

## ✅ Checklist
- [ ] Kod temiz ve okunabilir
- [ ] VDA standartlarına uygun
- [ ] Responsive tasarım korunmuş
- [ ] Dokümantasyon güncellenmiş
```

## 🎯 Katkı Alanları

### 🐛 Bug Fixes
- Form validasyon hataları
- JSON formatlaması sorunları
- Responsive tasarım sorunları
- Tarayıcı uyumluluk sorunları

### ✨ Yeni Özellikler
- Yeni VDA segmentleri
- Export formatları (XML, CSV)
- Import özelliği
- Template sistemi
- Batch işleme

### 🎨 UI/UX İyileştirmeleri
- Tasarım güncellemeleri
- Animasyonlar
- Accessibility iyileştirmeleri
- Mobil optimizasyonlar

### 📚 Dokümantasyon
- README güncellemeleri
- Kod dokümantasyonu
- Kullanım örnekleri
- Video tutoriallar

## 🏷️ Commit Mesajları

### Format:
```
type(scope): description

body (optional)

footer (optional)
```

### Tipler:
- `feat`: Yeni özellik
- `fix`: Bug düzeltmesi
- `docs`: Dokümantasyon
- `style`: Formatting, noktalama
- `refactor`: Kod refactoring
- `test`: Test ekleme
- `chore`: Build, config değişiklikleri

### Örnekler:
```
feat(715): add packaging dimensions validation
fix(export): resolve file download issue
docs(readme): update installation instructions
style(css): improve responsive design
```

## 📞 İletişim

- **GitHub Issues**: [Issues](https://github.com/ck-cankurt/vda4913-generator/issues)
- **Discussions**: [Discussions](https://github.com/ck-cankurt/vda4913-generator/discussions)
- **Email**: [Email](mailto:your-email@example.com)

## 🙏 Teşekkürler

Tüm katkıda bulunanlara teşekkürler! Bu proje açık kaynak topluluğunun desteği ile büyüyor.

---

**Not:** Bu rehberi takip ederek projeye değerli katkılar sağlayabilirsiniz. Herhangi bir sorunuz varsa lütfen iletişime geçin!
