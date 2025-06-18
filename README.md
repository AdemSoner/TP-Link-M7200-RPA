# TP-Link M7200 Modem RPA Otomasyon Projesi

Bu proje, TP-Link M7200 modeminin otomatik olarak yapılandırılmasını sağlayan bir RPA (Robotic Process Automation) çözümüdür. Modemde takılı olan **SIM kartı** ile sihirbaz kurulumunu tamamlar, enerji tasarrufu ayarlarını kapatır, Wi-Fi zamanlayıcısını devre dışı bırakır ve SMS kutusunu temizler.

## 🎯 Amaç

Manuel modem kurulum sürecini otomatikleştirerek zaman kazandırmak ve hatasız kurulum sağlamak.

## 🔧 Özellikler

- 📶 **Sihirbaz Kurulumu:** Otomatik olarak başlatılır ve tamamlanır.
- 🔋 **Power Saving Kapatma:** Modemin güç tasarrufu modu devre dışı bırakılır.
- 📡 **Wi-Fi Ayarlarını Kapatma:** Otomatik Wi-Fi zamanlayıcı özelliği kapatılır.
- ✉️ **SMS Kutusunu Boşaltma:** Gelen kutusu temizlenir.
- 💳 **SIM Desteği:** SIM kart üzerinden ağ kurulumu yapılır.

## 📁 Proje Dosyaları

| Dosya/Dizin           | Açıklama                                         |
|-----------------------|------------------------------------------------  |
| `main.xaml`           | Ana RPA betiği, tüm işlemleri sırasıyla yürütür  |
| `.screenshots/`       | Görsel tanıma için kullanılan ekran görüntüleri  |


## 🧰 Gereksinimler

- Windows işletim sistemi
- RPA aracı **UiPath**
- TP-Link M7200 modem ve Turkcell SIM
- Modem web arayüzüne erişim

## 🚀 Kurulum ve Kullanım

1. Modemi açın ve bilgisayara bağlayın.
2. UIPath Studio ile dizini açın veya direkt main.xaml dosyasını açın. 
3. Modem ilk kurulumda şifre zorunlu kıldığı için varsayılan olarak "sifre123" olarak ayarlıdır. Bunu değiştirmek için Studio'da main.xaml açıkken variables dan Password değişkenine değer vermeniz tavsiye edilir.
4. Direkt olarak F6 ile kurulum başlatılabilir veya publish alarak UIPathAssistant üzerinden robotu başlatıp izlenebilir.
5. Betik sırasıyla kurulumu başlatacak, gerekli ayarları yapacak ve SMS kutusunu boşaltacaktır.

> Not: Kurulum sırasında modem arayüzünün açık olması ve giriş bilgilerinin varsayılan olarak ayarlanmış olması beklenir.

## ⚠️ Uyarılar

- Bu proje yalnızca TP-Link M7200 modem ile test edilmiştir.
- SMS kutusunun silinmesi geri alınamaz; önemli mesajlar varsa lütfen yedekleyin.
- Otomasyon aracı, ekran görüntülerine göre işlem yapar. Web arayüz tasarımı değişirse betik güncellenmelidir.

## 📬 İletişim

Geri bildirim veya katkı için lütfen [GitHub üzerinden iletişime geçin](https://github.com/AdemSoner)