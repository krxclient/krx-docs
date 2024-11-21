---
icon: robot
---

# Fent Bot ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)
KRX İstemcisindeki **Fent Bot** sekmesi, yol bulma ve tünelleme yoluyla otomatikleştirme için gelişmiş bir araç sağlar.  
*Not: Botlardan kaçınırken, lütfen daha yüksek bir `cl_prediction_margin` kullanın [settings](../settings.md) bölümüne bakın ve ping'e göre tahmin marjını seçin*

---

## **Ekran Görüntüsü**
![Fent Bot Menüsü](https://raw.githubusercontent.com/Krixx1337/krxclient-docs/refs/heads/main/images/fentbot-menu.png)

---

## **Avoid**
- **Player Prediction**: Diğer oyuncuların hareketlerinin tahmin edilmesini sağlar.
- **Advanced Settings**: Botun davranışı için gelişmiş özelleştirme seçeneklerinin kilidini açar.
- **Use Skibidiforce**: Gelişmiş yol bulma için Skibidiforce algoritmasını etkinleştirir.
  - **Skibidiforce Depth**: Skibidiforce hesaplamalarının derinliğini yapılandırır.
- **Fent Ticks**: Fent tabanlı yol bulma için tik süresini tanımlar.
- **Tweaker Inputs**: Ayarlayıcı girişlerinin sayısı.
- **Tweaker Ticks**: Tweaker girişleri için tik süresini ayarlar.
- **Inject Fent**: Taramayı başlatmak için tek tıklama eylemi.  

## **Misc**
- **Skibidiforce Aim Points**: Skibidiforce tarafından kullanılan hedef noktalarının sayısını yapılandırır.
- **Render Path**: Hesaplanan yolu görsel olarak görüntüler.
- **Render Tunnels**: Yol bulma için kullanılan tünelleri vurgular.
- **Spectate Scan**: Tarama sırasında ilerleme taramasının izlenmesini sağlar.  
- **Tunnel Editor**: Tünelleri manuel olarak özelleştirmek için bir kullanıcı arayüzü sağlar.
- **Auto Tunnels**: Yüklenen bir yeniden oynatmadan optimize edilmiş hareket için otomatik olarak tüneller oluşturur.
- **Tunnel Width**: Otomatik olarak oluşturulan tünellerin genişliğini ayarlar.
- **Clear Tunnels**: Tüm tünelleri kaldırır.

---

## **Configuration**
- Çoğu zaman KRX tarafından sağlanan varsayılan ayarları kullanmak yeterlidir. İşte iyi CPU'lara sahip daha ileri düzey kullanıcılar için olası bir yapılandırma:
- **Player Prediction**: KAPALI
- **Advanced Settin*gs*: AÇIK
- **Use Skibiforce**: AÇIK
- **Skibidiforce Width**: 4
- **Fent Ticks**: 1000
- **Tweaker Inputs**: maksimum
- **Tweaker Ticks**: 4-8
