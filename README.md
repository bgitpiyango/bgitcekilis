# Betgit Piyango Çekiliş Sistemi

Betgit Piyango Çekiliş Sistemi, WordPress tabanlı güvenli ve şeffaf bir çekiliş eklentisidir. Bu eklenti ile sitenizde rastgele çekilişler düzenleyebilir, kazananları belirleyip veritabanında güvenle saklayabilirsiniz. 

---

### Özellikler

- **Güvenli Rastgelelik:**  
  PHP’nin `random_int()` fonksiyonunu kullanarak, sunucu tarafında kriptografik olarak güvenli ve benzersiz rastgele sayılar üretir.

- **Şeffaflık ve Doğrulama:**  
  Eklenti dosyanızın SHA-256 hash değeri hem kullanıcıya hem de CSV çıktısında gösterilir. Bu sayede çekiliş sonuçlarının ve dosyanın doğruluğu kolaylıkla kontrol edilebilir.

- **Kolay Yönetim:**  
  WordPress yönetici panelinden çekiliş kazananlarını listeleyebilir, sayfalayabilir, CSV olarak dışa aktarabilir ve veritabanını sıfırlayabilirsiniz.

- **Kullanıcı Dostu Arayüz:**  
  Özel tasarlanmış butonlar ve dinamik sonuç kartlarıyla çekiliş sürecini zahmetsizce yönetin.

- **Kazanan Listesi:**  
  DataTables entegrasyonu ile kazananları filtreleyip arayabilir, sütun bazlı sorgulamalar yapabilirsiniz.

---

### Kurulum

1. **Eklentiyi Yükleyin:**
   - Bu repoyu indirin ve WordPress kurulumunuzda `wp-content/plugins/` dizinine yükleyin.
   
2. **Eklentiyi Etkinleştirin:**
   - WordPress yönetici paneline gidin.
   - "Eklentiler" bölümünden **Betgit Piyango Çekiliş Sistemi** eklentisini bulun ve etkinleştirin.
   - Eklenti etkinleştirilirken gerekli veritabanı tabloları otomatik olarak oluşturulacaktır.

---

### Kullanım

- **Çekiliş Başlatma:**
  - Bir sayfa veya yazı oluşturun ve içine `[cekilis_yap]` kısa kodunu ekleyin.
  - Bu kısa kod, ziyaretçilerinizin çekiliş yapabilmesi için gerekli arayüzü oluşturur.

- **Kazananların Listesi:**
  - Bir başka sayfada veya yazıda `[kazanan_listesi]` kısa kodunu kullanarak kazananların listesini görüntüleyin.
  - Bu liste, DataTables entegrasyonu ile gelişmiş filtreleme ve arama özelliklerine sahiptir.

- **CSV Olarak Dışa Aktarma:**
  - Yönetici panelinde "Çekiliş Yönetimi" sayfasından "CSV Olarak Dışa Aktar" butonuna tıklayın.
  - İndirilen CSV dosyasının başında eklentinin SHA-256 hash değeri yer alır; bu, dosyanın eklenti ile üretildiğini doğrular.

- **Veritabanını Sıfırlama:**
  - Yönetici panelinde "Çekiliş Yönetimi" > "Veritabanını Sıfırla" seçeneğini kullanarak tüm çekiliş verilerini temizleyebilir ve sıfırlayabilirsiniz.

---

### Güvenlik ve Şeffaflık

- **Kod Bütünlüğü:**  
  Eklenti dosyasının SHA-256 hash değeri, kullanıcıya ve CSV çıktısına yansıtılarak dosyanın bütünlüğü ve doğruluğu sağlanır.

- **Güvenli Veri İşlemleri:**  
  Tüm rastgele sayı üretimleri sunucu tarafında, nonce ve yetkilendirme kontrolleriyle korunarak gerçekleştirilir. Bu sayede çekiliş süreçleri güvenle yürütülür.

---

### Katkıda Bulunma

Geliştirmeler, hata düzeltmeleri veya yeni özellik önerileri için projeyi forklayarak katkıda bulunabilirsiniz. 

---

**Sürüm:** 2.9.2  


Kod Bütünlüğü:
Dosya Hash (SHA-256): 1d48cb23353e4f45b244ceb1304ab6581210eccce50d805167d18386f457866e

Hash Oluşturulma Tarihi: 13.01.2025 14:54:30
