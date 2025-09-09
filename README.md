# Fotoğraf Yazdırma ve Sayfa Düzeni Aracı (Photo Print Layout Tool)

[![Lisans: MIT](https://img.shields.io/badge/Lisans-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Birden fazla fotoğrafı tek bir A4 sayfasına otomatik olarak yerleştirerek kolayca yazdırmanızı sağlayan basit ve sunucusuz bir web aracı.

![Uygulama Ekran Görüntüsü]

<img width="677" height="1300" alt="Screen Shot 2025-09-09 at 23 23 31" src="https://github.com/user-attachments/assets/55258d85-8f0a-4c22-b55a-6051e58b9b2f" />


## 📝 Açıklama

Bu araç, birden çok fotoğrafı (vesikalık, anı fotoğrafı vb.) tek bir A4 kağıdına en verimli şekilde sığdırma problemini çözmek için geliştirilmiştir. Photoshop veya benzeri karmaşık yazılımlara ihtiyaç duymadan, sadece tarayıcınızı kullanarak fotoğraflarınızı seçin, aracın otomatik olarak en uygun sayfa düzenini oluşturmasını izleyin ve yazdırın. Tüm işlemler tamamen sizin tarayıcınızda (istemci tarafında) gerçekleşir, bu sayede fotoğraflarınız gizli ve güvende kalır.

## ✨ Temel Özellikler

*   **Çoklu Fotoğraf Yükleme:** Tek seferde birden fazla fotoğraf dosyası seçin.
*   **Otomatik Sayfa Düzeni:** Seçilen fotoğraf sayısına göre en uygun grid (ızgara) düzenini (1x1, 2x2, 2x3, 3x4 vb.) otomatik olarak oluşturur.
*   **A4 Optimizasyonu:** Düzenler, standart A4 kağıt boyutuna maksimum verimlilikle sığacak şekilde tasarlanmıştır.
*   **Canlı Önizleme:** Yazdırma işleminden önce fotoğraflarınızın A4 sayfasında nasıl görüneceğini net bir şekilde görün.
*   **Sunucusuz Çalışma:** Hiçbir sunucuya veya internet bağlantısına ihtiyaç duymaz. Tüm işlemler JavaScript ile tarayıcıda yapılır.
*   **Mobil Uyumlu:** Telefon ve tablet gibi mobil cihazlarda da sorunsuz çalışır ve yazdırma işlemini destekler.
*   **Kolay Kullanım:** "Fotoğraf Seç", "Yazdır" ve "Temizle" butonları ile basit ve sezgisel bir arayüze sahiptir.

## 🚀 Nasıl Kullanılır?

1.  **Repo'yu Klonlayın veya İndirin:**
    ```bash
    git clone https://github.com/furkngld/photo-print-tool.git
    ```
2.  **`index.html` Dosyasını Açın:** Proje klasöründeki `index.html` dosyasına çift tıklayarak aracı tarayıcınızda çalıştırın.
3.  **Fotoğraf Seçin:** <kbd>Fotoğraf Seç</kbd> butonuna tıklayarak bilgisayarınızdan veya telefonunuzdan yazdırmak istediğiniz fotoğrafları seçin.
4.  **Önizlemeyi Kontrol Edin:** Seçtiğiniz fotoğraflar için oluşturulan sayfa düzeni önizlemesini kontrol edin.
5.  **Yazdırın:** <kbd>Yazdır</kbd> butonuna tıklayarak tarayıcının yazdırma diyalogunu açın ve yazdırma işlemini başlatın.

## 🛠️ Teknik Detaylar

*   **Frontend:** HTML5, CSS3, ve Vanilla JavaScript (hiçbir kütüphane veya framework kullanılmamıştır).
*   **Dosya Okuma:** `FileReader API`, kullanıcı tarafından seçilen resim dosyalarını yerel olarak okumak ve base64 formatına dönüştürmek için kullanılır.
*   **Dinamik Düzen Oluşturma:** JavaScript, seçilen fotoğraf sayısına göre DOM'u dinamik olarak manipüle ederek hem önizleme alanını hem de yazdırma için gizli olan (`#print-area`) bölümü oluşturur.
*   **Yazdırma Stilleri:** `@media print` CSS kuralları, sadece yazdırma işlemi sırasında aktif hale gelerek sayfa kenar boşluklarını sıfırlar, gereksiz arayüz elemanlarını gizler ve fotoğraf grid'ini A4 sayfasına tam olarak sığdırır.
*   **Grid Sistemi:** Fotoğrafların yerleşimi için modern `CSS Grid Layout` kullanılmıştır.

## 🤝 Katkıda Bulunma

Katkılarınız projeyi daha iyi hale getirecektir! Lütfen bir "issue" açarak hata bildiriminde bulunun veya yeni özellikler önerin. "Pull request" göndermekten çekinmeyin.

1.  Projeyi Fork'layın.
2.  Kendi branch'inizi oluşturun (`git checkout -b ozellik/yeni-bir-ozellik`).
3.  Değişikliklerinizi commit'leyin (`git commit -m 'Yeni bir özellik eklendi'`).
4.  Branch'inizi push'layın (`git push origin ozellik/yeni-bir-ozellik`).
5.  Bir Pull Request açın.

## 📜 Lisans

Bu proje [MIT Lisansı](https://opensource.org/licenses/MIT) ile lisanslanmıştır.
