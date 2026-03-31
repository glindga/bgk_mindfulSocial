mindfulSocial - Ürün Gereksinim Belgesi
1. Ürün Vizyonu ve Özeti
mindfulSocial, kullanıcıların sosyal medya (Instagram vb.) üzerindeki kontrolünü geri kazanmasını sağlayan yapay zeka destekli bir tarayıcı eklentisidir.
Algoritmaların dikkat dağıtıcı görsel gücünü kırarak, kullanıcıya içeriği tüketmeden önce "bilinçli bir tercih" yapma şansı sunar.

2. Hedef Kitle ve Kullanıcı İhtiyaçları
Dijital Minimalistler: Sosyal medyada sadece ihtiyacı olan bilgiye ulaşmak isteyenler.

Odaklanma Sorunu Yaşayanlar: Görsel uyaranlar nedeniyle "doomscrolling" döngüsüne giren bireyler.

Öğrenciler ve Profesyoneller: Çalışma sırasında sosyal medyayı bir iletişim aracı olarak kullanırken dikkati dağılanlar.

3. Fonksiyonel Gereksinimler (Functional Requirements)
FR1: İçerik Maskeleme (Shielding)
Sistem, Instagram akışındaki görselleri/videoları otomatik olarak kapatmalıdır.

Maskeleme, orijinal içeriğin üzerine bir "Kalkan Katmanı" eklenerek yapılmalıdır.

FR2: AI Tabanlı Multimodal Özetleme
Kullanıcı "Summarize" butonuna bastığında, sistem gönderinin görselini ve metnini Gemini 3 Flash API'ye göndermelidir.

AI, içeriği analiz ederek maksimum 2 cümlelik objektif bir özet sunmalıdır.

FR3: Duygu ve İçerik Analizi
Sistem, içeriğin duygu durumunu (Pozitif, Negatif, Nötr) analiz etmelidir.

İçerikle ilgili en alakalı 3 anahtar kelimeyi (Etiket) üretmelidir.

FR4: İsteğe Bağlı İçerik Gösterimi (View Content)
Kullanıcı özeti okuduktan sonra içeriği görmek isterse, "View Content" butonu ile maskeyi kaldırabilmelidir.

4. Teknik Gereksinimler (Technical Requirements)
Platform: Google Chrome (Manifest V3).

API Entegrasyonu: Google Gemini 3 Flash (Multimodal destekli).

Veri Güvenliği: Kullanıcının API anahtarı sadece yerel tarayıcı depolama alanında (chrome.storage.local) tutulmalıdır.

Performans: AI özetleme işlemi 3 saniyenin altında tamamlanmalıdır.

5. Başarı Metrikleri (KPIs)
Odaklanma Oranı: Kullanıcıların akışta geçirdiği toplam sürenin, eklenti öncesine göre azalması.

Seçici Tüketim: Özetlenen içeriklerin sadece %50'sinden azının "View Content" ile açılması (Kullanıcının sadece gerçekten ilgisini çeken içeriğe bakması).

Hata Payı: AI özetlerinin kullanıcı tarafından "doğru" olarak değerlendirilme oranı.

6. Gelecek Yol Haritası (Future Roadmap)
Platform Genişletme: TikTok ve Twitter (X) desteği.

Hata Yönetimi Geliştirme: API tarafında oluşan "Unterminated string" gibi parse hatalarının otomatik onarılması.

Kullanım İstatistikleri: Kullanıcıya haftalık olarak kaç adet "gereksiz" içeriği engellediğini gösteren bir dashboard.
