# Kullanıcı Deneyim Akışı (User Flow)

1. **Kurulum:** Kullanıcı eklentiyi yükler ve Gemini API anahtarını popup üzerinden kaydeder.
2. **Aktivasyon:** Kullanıcı Instagram'a girdiğinde eklenti otomatik olarak çalışır.
3. **Kalkan Modu:** Akıştaki tüm gönderiler koyu renkli bir kalkan kartı ile kaplanır. Orijinal görsel/video gizlenir.
4. **Etkileşim:** Kullanıcı bir gönderiyi merak ederse kartın üzerindeki "AI ile Özetle" butonuna tıklar.
5. **Analiz Süreci:** - Eklenti, arka planda gönderinin görselini ve açıklamasını yakalar.
    - Veriler Gemini API'ye gönderilir.
    - "Analiz ediliyor..." animasyonu gösterilir.
6. **Sonuç:** Kalkanın üzerinde kısa bir özet, 3 anahtar kelime ve içerik duygu durumunu belirir.
7. **Karar:** Kullanıcı özete göre içeriği tamamen açabilir veya kaydırıp geçebilir.
