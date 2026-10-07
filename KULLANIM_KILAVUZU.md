# 🐄 Sığır Sağlık Rehberi - Kullanım Kılavuzu

**Sığır Sağlık Rehberi**, internet bağlantısı ve sunucu kurulumu gerektirmeyen, doğrudan telefon ve bilgisayar tarayıcısında çalışan, Progressive Web App (PWA) mimarisine sahip %100 çevrimdışı bir büyükbaş sürü sağlığı, besi ve süt yönetim asistanıdır.

---

## 🚀 1. Hızlı Başlangıç & PWA Kurulumu

### Telefonunuza Yükleme (Android / iOS):
1. İnternet bağlantınız varken **[https://mserman90.github.io/sigir-saglik-rehberi/](https://mserman90.github.io/sigir-saglik-rehberi/)** adresine gidin.
2. Tarayıcı menüsünden (üç nokta veya paylaş butonu) **"Ana Ekrana Ekle"** veya **"Uygulamayı Yükle"** seçeneğine dokunun.
3. Telefonunuzun ana ekranına uygulama simgesi eklenir. Artık dağda, merada, internetin ve baz istasyonunun hiç çekmediği bodrum ahırlarda dahi tam ekran ve ultra hızlı çalışır.

### Bilgisayarda Açma:
- Doğrudan web adresini açabilir veya depodaki [`index.html`](./index.html) dosyasına çift tıklayarak herhangi bir tarayıcıda çalıştırabilirsiniz.

---

## 🧭 2. Butonlar & Menü Öncelik Düzeni

Uygulama menüleri, ahır ve mera koşullarındaki **klinik aciliyet** ve **günlük kullanım sıklığına** göre optimize edilmiştir:
- **Alt Menü (Bottom Navigation):** Başparmakla kolay erişim için `📊 Ahır Özeti` $\rightarrow$ `🆘 İlk Yardım` $\rightarrow$ `🩺 Muayene` $\rightarrow$ `💊 İlaç & Süt` $\rightarrow$ `🥛 Sağımcı` $\rightarrow$ `🌾 Yem & Geviş` $\rightarrow$ `🍼 Buzağı` $\rightarrow$ `🚛 Dana Giriş` $\rightarrow$ `⚖️ Kilo/CAAG` $\rightarrow$ `🩸 Tohum/Doğum` $\rightarrow$ `📅 Aşı Takvimi` $\rightarrow$ `💰 Zarar Defteri` sırasında dizilmiştir.
- **Hızlı İşlemler Paneli:** Hayat kurtaran `🆘 Acil İlk Yardım` en üstte çift genişlikli buton olarak konumlandırılmıştır.
- **Eldiven & Saha Uyumu:** Tüm butonlar en az 48px dokunma yüksekliğine sahip olup eldivenli, ıslak ve güneşli/karanlık saha şartlarına uygundur.

---

## 📱 3. Temel Modüller ve Kullanım Rehberi

### 0. 📷 Kamerayla Küpe Okuma (Barkod / QR)
- Hayvan arama, muayene, ilaç yapma, tohumlama, tartım ve sağım ekranlarında yer alan sarı **"📷 Oku"** butonuna basın.
- Kamerayı hayvanın sarı kulak küpesindeki barkod veya karekoda doğrultun.
- Küpe numarası otomatik doldurulur, telefon hafifçe titrer ve ilgili hayvanın sağlık kaydı ekrana gelir.

---

### 1. 📊 Ahır Özeti & Hayvan Kaydı
- **Yeni Hayvan Ekleme:** Ekrandaki **"+ Yeni Ekle"** butonuna basarak küpe numarası, cinsiyeti, yaşı ve et-yağ kondisyon durumunu girin.
- **Pazardan / Kamyondan Yeni Gelenler:** *"Pazardan yeni alındı, ayrı bölmede bekleyecek (Karantina)"* kutucuğunu işaretlerseniz sürüye hastalık bulaşmaması için sistem hayvanı sarı alarm durumuna alır.
- **Hayvan Silme:** Listeden satırın sonundaki *"Sil"* butonuna basarak kaydı silebilirsiniz.

---

### 2. 🆘 Acil İlk Yardım & Besi Hastalıkları Müdahalesi
Veteriner hekim ahıra ulaşana kadar hayat kurtaracak ilk adımlar:
- **⚖️ Canlı Ağırlık Doz Hesaplayıcı:** Kilosu girildiğinde anafilaktik şok için hayat kurtaran Adrenalin dozunu (1:1000 Adrenalin, her 45 kg için 1 mL) anında hesaplar.
- **💉 İğne / Aşı Şoku (Anafilaksi):** İlacı derhal kesme, hesaplanan dozu vurma ve hava yolu açma talimatı.
- **🎈 İşkembe Şişmesi & Gaz Patlaması (Timpani):** Sol boşluk kontrolü, hortum salma, köpük varsa bitkisel sıvı yağ içirme ve acil durumlarda sol açlık çukurundan trokar (şişleme) tekniği.
- **🔴 Rahim Çıkması / Düşmesi (Prolapsus):** Döl yatağını pisliğe değdirmeme, ılık temiz tuzlu bezle yukarı kaldırma ve ineğin arkasını samanla yüksekte tutma.
- **📉 Doğum Felci (Süt Humması / Kalsiyum Çökmesi):** Damardan çok yavaş kalsiyum serumu (en az 15–20 dk) ve ineği oturur vaziyette tutma uyarısı.
- **🥔 Yemek Borusu Tıkanması (Patates/Pancar Boğulması):** Boğazı sıvazlayarak yukarı alma, sert hortum itmeme ve gaz boğulmasını önleme.
- **🩸 Şiddetli Kanama & Boynuz/Tırnak Kırılması:** Basınçlı tampon, boynuz kökü bağlama ve atardamar turnikesi.
- **🍼 Yeni Doğan Buzağıyı Canlandırma:** Balgam temizliği, kısa süreli baş aşağı tahliye, soğuk su ve saman çöpü şoku.
- **☀️ Sıcak Çarpması & Hararet:** Boyun damarlarından ve bacaklardan soğutma, serin su ve tuzlu-pekmezli can suyu desteği.
- **☠️ Zehirlenme & Gübre / Üre Yutma:** Üre gübresi yutulmuşsa sulandırılmış ev sirkesi içirme, zehirli ot için aktif kömür ve sıvı yağ desteği.
- **🧠 CCN / Polio (Besi Danası B1 Eksikliği):** Aşırı arpa/asidoz sonrası kafayı sırtına bükme ("yıldız gözleme") belirtisinde acil damar ve kas içi B1 Tiamin hayat kurtarır.
- **💧 İdrar Taşı & Sidik Zoru (Ürolitiyazis):** Kalsiyum-fosfor dengesizliği veya susuzlukta penisi tıkayan taşlarda sidik torbası patlamadan önce ağrı kesici ve rasyona Amonyum Klorür / tuz desteği.
- **🦶 Besi Laminitisi (Arpa Vurması / Ayak Yanması):** Fazla arpa yenmesi sonrası tırnak felcinde yemliği boşaltma, ağızdan karbonat, fluniksin ve tırnaklara 20-30 dk soğuk su banyosu.

---

### 3. 🩺 Hasta Hayvan Kontrolü & Muayenesi (Saha Triyajı)
Bir ineğin hastalandığından şüphelendiğinizde:
1. **Makat Ateşi (°C):** Dereceyle ölçtüğünüz ateşi yazın (Normal: 38.0–39.3 °C. 39.5 °C ve üzeri kırmızı alarmdır).
2. **Nabız & Nefes:** 1 dakikadaki kalp atımı ve nefes sayısını girin.
3. **İşkembe Çalışması:** Sol açlık çukurunu dinleyip dalga sayısını seçin.
4. **Hastalık Puanlama (DART):** Keyifsizlik, iştah durumu ve hırıltılı nefes seçeneklerini 0'dan 3'e kadar işaretleyin.
5. Sistem anında **"DURUMU İYİ"**, **"ORTA DERECE HASTA (İlaç Lazım)"** veya **"ÇOK ACİL & AĞIR HASTA (Veterineri Çağır)"** kararı verir ve ne yapmanız gerektiğini maddeler halinde sıralar.

---

### 4. 💊 İlaç Kaydı & Sütü/Eti Tanka Yasaklama (İKAS)
Antibiyotik veya iğne yaptığınızda süt ve etin tanka karışmasını önler:
1. İlaç yapılan hayvanı ve uygulanan ilacı listeden seçin.
2. Vurulan dozu ve saati onaylayıp kaydedin.
3. Sistem yasal arınma süresine göre (Merck Vet standartları) **saat ve dakika bazında geri sayım** başlatır.
4. **Kombine Kuralı:** Hayvana aynı gün 2 farklı ilaç yapıldıysa sistem otomatik olarak süresi en uzun olan ilacın gününü kilitler.

---

### 5. 🥛 Sağımcı Ekranı (Büyük Puntolu Hızlı Kontrol)
Sağımhanede çalışan personelin tek bakışta görmesi için hazırlanmıştır:
- Küpe numarasını yazın veya kamerayla okutun.
- Eğer hayvana antibiyotik vurulmuşsa ekran **kocaman kırmızı alarm** verir ve kaç saat kaldığını gösterir.
- İlaçsız ineklerde **"🟢 SAĞIMA UYGUN"** yeşil onayı çıkar.
- Mezbahaya gönderilmesi yasak olan kesim kilitli hayvanlar anlık listelenir.

---

### 6. 🌾 Yemlik Düzeni, İşkembe Sağlığı & Geviş Sayacı
1. **Geviş Getirme Sayacı:** Yem döküldükten 2 saat sonra ahırdaki yerde yatan inekleri ve geviş getirenleri sayıp yazın. Hedef en az %58-60'tır. Altında kalırsa işkembe ekşimesi (asidoz) uyarısı verir.
2. **Tezek Kıvamı (1-5):** Tezeğin cıvıklığına bakarak rasyondaki saman veya fabrika yemi dengesini test edin.
3. **Karbonat Dozu:** Sağılan inek sayısını girerek yem karma makinesine kaç kilo sodyum bikarbonat katmanız gerektiğini otomatik hesaplayın.

---

### 7. 🍼 Buzağı Hayatta Tutma & İlk Ağız Sütü (Kolostrum)
1. **Altın Kural:** Doğumdan sonraki **ilk 2 saat içinde** ananın koyu ağız sütünden en az 3–4 litre mutlaka içirilmelidir!
2. **Brix Kalite Ölçer:** Işıklı optik camla (refraktometre) ölçülen yüzdeyi girin. %22 ve üstü mükemmel kalitedir.
3. **Buzağı İshali: Su Kaybı (Kuruma) & Damar/Ağız Serumu Hesabı:** Buzağının kilosunu ve göz çökme derecesini seçin. 24 saatte kaç litre ağızdan ishal tozu / can suyu veya damardan serum verilmesi gerektiği anında hesaplanır.
4. **Göbek Kordonu Dezenfeksiyonu:** Doğum anında ve 1-2 saat sonra %7'lik tentürdiyota tamamen daldırma kontrol listesi.

---

### 8. 🚛 Yeni Dana Giriş & Besiye Alıştırma Protokolü
Kamyondan veya pazardan yeni gelen danaların nakliye şokunu, yol hummasını (Shipping Fever / BRD) ve asidozu önlemek için geliştirilmiş 21 günlük protokol:
1. **1. Gün Kamyondan İniş:** İlk 2 saat su tekneleri kapalı tutulur, sadece kuru ot/saman verilir. 2 saat sonra ılık **tuzlu-pekmezli can suyu** içirilir; kesif yem ve aşı kesinlikle verilmez!
2. **Metafilaksi & Aşı Planı:** Yüksek riskli danalara Tulatromisin koruyucu ciğer iğnesi dozu, iç-dış parazit iğnesi ve AD3E vitamin desteği hesaplanır.
3. **21 Günlük Yem Geçiş Tablosu:** Samandan arpa/kesif yeme geçiş kademe kademe yönetilir.

---

### 9. ⚖️ Canlı Kilo & Besi CAAG Takip Motoru
1. **Kantar veya Şerit Metre:** İster baskül ağırlığını girin, ister baskül yokken şerit metreyle göğüs ve boy ölçüsünü girerek bilimsel *Schaeffer Formülü* ile kilo hesaplayın.
2. **CAAG (Günlük Canlı Ağırlık Artışı):** İki tartım arasındaki günlük kilo alım hızını (hedef: 1.2–1.4 kg/gün) hesaplar.
3. **Karkas & Gelir Projeksiyonu:** Tahmini randıman (%58), karkas et ağırlığı ve mezbaha satış geliri tek tıkla listelenir.

---

### 10. 🩸 Tohumlama, Gebelik & Doğum Çarkı
1. Tohumlanan ineği, tarihi ve boğa kodunu kaydedin.
2. Otomatik zaman çizelgesi hesaplanır:
   - **21. Gün:** Kızgınlık dönüş kontrolü.
   - **40. Gün:** Ultrason / rektal gebelik muayenesi.
   - **220. Gün:** Kuruya alma ve kuru dönem tüpü (Doğuma 60 gün kala).
   - **280. Gün:** Beklenen doğum günü.

---

### 11. 📅 Akıllı Aşı Takvimi & Hatırlatıcı
- Şap (FMD), Bruselloz (S19), Çiçek (LSD), BRD karma solunum ve Buzağı İshali aşıları.
- Rapel (tekrar) tarihlerini otomatik hesaplar (21 gün ve 30 gün kuralı).
- TÜRKVET resmi kayıt ve 21 gün sevk kuralını hatırlatır.

---

### 12. 💰 Hastalık Masrafı & Dökülen Süt Zarar Defteri
Hastalıkların çiftliğinize gerçek ekonomik maliyetini kuruşu kuruşuna gösterir:
1. Çiğ süt satış fiyatınızı (Örn: 16.5 TL/Litre) yazın.
2. Tedavi gören hayvanı, hastalığını, veteriner ve ilaç masrafını girin.
3. İlaç yüzünden lavaboya dökülen günlük süt miktarını ve kaç gün döküldüğünü yazın.
4. Toplam maliyeti ve dökülen sütün parasal zararını deftere kaydeder.

---

## 💾 4. Veri Yedekleme & Telefona Aktarma
- Sağımcı ekranının en altında yer alan **"📥 Yedeği İndir (JSON)"** butonuna basarak tüm hayvan, muayene, tartım, geliş ve aşı kayıtlarınızı tek bir yedek dosyası olarak indirebilirsiniz.
- Başka bir telefona geçtiğinizde **"📤 Yedeği Yükle"** diyerek saniyeler içinde tüm çiftlik verilerinizi geri yükleyebilirsiniz.
- Tüm veriler telefonunuzun kendi güvenli hafızasında tutulur; internete bağımlı değildir.
