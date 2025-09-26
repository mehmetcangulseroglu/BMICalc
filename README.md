# BMI Hesaplayıcı

Bu uygulama, kullanıcıların Vücut Kitle İndeksi (BMI) hesaplamalarını kolayca yapmalarını sağlayan basit bir grafik arayüz uygulamasıdır.

## Özellikler

- Kullanıcı dostu grafik arayüz
- Kilo ve boy girişi için input alanları
- Otomatik BMI hesaplama
- BMI değerine göre sağlık durumu kategorilendirmesi
- Hata kontrolü ve kullanıcı uyarıları

## BMI Kategorileri

| BMI Değeri | Kategori |
|------------|----------|
| < 18.5     | Zayıf    |
| 18.5 - 24.9| Normal   |
| 25.0 - 29.9| Fazla Kilolu |
| ≥ 30       | Obez     |

## Gereksinimler

- Python 3.x
- tkinter (Python ile birlikte gelir)

## Kurulum

1. Python'un bilgisayarınızda kurulu olduğundan emin olun
2. Proje dosyasını indirin
3. Terminalde proje dizinine gidin

## Kullanım

```bash
python bmi_hesaplayici.py
```

### Kullanım Adımları

1. Uygulamayı çalıştırın
2. Kilo alanına kilonuzu kg cinsinden girin
3. Boy alanına boyunuzu metre cinsinden girin (örn: 1.75)
4. "Hesapla" butonuna tıklayın
5. Sonucu ekranda görüntüleyin

## Kod Yapısı

### Ana Fonksiyon: `bmi_hesapla()`

- Kullanıcı girişlerini alır ve doğrular
- BMI hesaplamasını yapar: `BMI = Kilo / (Boy²)`
- Sonucu kategorize eder
- Hata durumlarını yönetir

### Hata Kontrolü

- Boş alan kontrolü
- Sayısal değer kontrolü
- Pozitif sayı kontrolü
- ValueError exception handling

### GUI Bileşenleri

- **Entry**: Kilo ve boy girişi için
- **Label**: Başlıklar ve sonuç gösterimi için
- **Button**: Hesaplama tetikleyici
- **messagebox**: Uyarı ve hata mesajları

## Önemli Notlar

- Boy metre cinsinden girilmelidir (1.75 gibi)
- Kilo kg cinsinden girilmelidir
- Sadece pozitif sayılar kabul edilir
- Tüm alanların doldurulması zorunludur

## Geliştirme Notları

- Tüm işlemler fonksiyon içinde yapılmıştır
- Button command parametresi için fonksiyon referansı kullanılmıştır (parantez olmadan)
- Exception handling ile güvenli kullanıcı deneyimi sağlanmıştır

## Lisans

Bu proje eğitim amaçlı hazırlanmıştır ve özgürce kullanılabilir.
