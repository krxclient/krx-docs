---
icon: sparkles
---

# **Misc**

**Misc** sekmesi, oynanışı geliştirmek, koruma sağlamak ve eğlenceli trolleme mekaniklerini etkinleştirmek için tasarlanmış özellikler sunar.

---

## **Ekran Görüntüsü**
![Misc Menu](https://raw.githubusercontent.com/Krixx1337/krxclient-docs/refs/heads/main/images/misc-menu.png)

---

## **Features**

### **Bots**
- **Moonwalk**: Oyuncunun hem sol hem de sağ tuşlara basarken hareket yönünü ileri geri değiştirerek “Moonwalk” yapmasını sağlar.
- **Auto Fire**: Ateş düğmesine basılı tuttuğunuzda silahınız otomatik olarak ateş eder.
- **Auto Rehook**: Bir oyuncuyu başarıyla tuttuktan sonra, kanca düğmesini basılı tutmaya devam ederseniz, otomatik olarak yeniden tutmaya çalışır.
- **Auto Jump Save**: Donmayı önlemek için otomatik olarak zıplar.
- **Quick Stop**: Oyuncunun mevcut hızına karşı hareket yönünü ayarlayarak oyuncuyu hızlı ve sorunsuz bir şekilde durdurur.
- **Avoid Freeze**: Sol/sağ yaparak donmayı önlemeye yardımcı olur.  
- **Dummy Fly**: Kuklanız otomatik olarak sizinle birlikte Dummy Flyyapar ve Dummynize çekic ve kancada attırır. ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)  
- **Jet Ride**: Hook ride botunun jetpackli hali. A/W/S/D tuşlarıyla kontrol edilir. ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)  
- **Auto Aled**: Aled mümkünse otomatik çekiç vurur. ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)  

### **Protections**
- **Random Timeout Seed**: Parmak izini önlemek için bir sunucuya bağlanmadan önce yeni bir zaman aşımı seedi oluşturur. Not: Bu özellik etkinken zaman aşımına uğradıktan sonra eski konumunuza tekrar dönemezsiniz.
- **Version Spoof**: Kısıtlamaları atlamak için istemci sürümünü/Kimliğini değiştirir. Emin değilseniz kapalı bırakın.

### **Mod Dedector**  
- **Enable**: Sunucudaki potansiyel yetkilileri veya şüpheli oyuncuları belirlemek için Yetkili Dedektörü özelliğini açar.  
- **Detect by Names**: Bilinen yetkililer için oyuncu adlarını tarar.
- **Detect Suspicious Players**: Potansiyel yetkilileri veya sizi rapor edebilecek oyuncuları tespit etmek için oyuncu adlarını tarar.  
- **Leave on Mod Detection**: Bir yetkili tespit edilirse sunucu ile olan bağlantıyı otomatik olarak keser.
- **Leave on Warn Detected**: Sizi rapor edebilecek potansiyel bir yetkili veya oyuncu tespit edilirse sunucu bağlantısını otomatik olarak keser. 
### **Auto Unfreeze** ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)
- **Enable**: Otomatik Auto Unfreeze özelliğini etkinleştirir, bu özellik donduğunuzda kurtulabilir bir pozisyondaysanız size otomatik lazer atar.
- **Advanced Settings**: Ayrıntılı kontrol için daha ayrıntılı yapılandırma seçeneklerini etkinleştirir.
    - **Bounces**: Lazerin duvarlardan nasıl sekeceğini belirler:
        - **Least**: En az sekmenin olduğu bir yön seçerek daha hızlı çözülme sağlar.
        - **Most**: En çok sekmenin olduğu yönü seçer. TAS senaryolarında kullanışlıdır, çünkü daha uzun sekmeler mermileri daha hızlı yeniden doldurur.
    - **Silent**: Bu ayarı kullandığınızda nişangahınız aim etkilerinden etkilenmez.
    - **Points**: Kurtarılma yönlerini kontrol ederken dikkate alınan nokta sayısını yapılandırır. Daha yüksek değerler daha hassas kontroller sağlar.
    - **Current Dir Ticks**: Geçerli yönü hesaplamak için lazerin kaç tick kullanılacağını ayarlar. Daha iyi doğruluk için ayarlayın.
    - **Ticks**: En iyi kurtarma yönü belirlenirken lazerin kaç tick analiz edileceğini tanımlar.
    - **FOV**: Lazerin hedefleme menzilini belirlemek için görüş alanını ayarlar.

### **Fake Aim**
- **Enable**: Diğer oyuncuların kafasını karıştırmak veya yanıltmak için sahte aim açar.
- **Send Always**: Etkinleştirilirse, hedefin yönü her tickte sunucuya gönderilir (diğerleri için daha düzgün görünür).
- **Visible**: Sahte aimi ekranınızda gösterir.
- **Modes**: Sahte aimin nasıl davranacağını belirler:
  - **Mouse Pos**: Hedefinizi fare konumunuzu takip edecek şekilde ayarlayarak gores bot aimbot'un daha az belirgin görünmesini sağlar.
  - **Robot Aim**: Aim pozisyonunuzu sadece kanca atarken veya ateş ederken gösterir.
  - **Spinbot**: Hedefinizi bir dönme hareketiyle hızla döndürür.
  - **Random**: Teenizi çok hızlı bir şekilde döndürür.
  - **Fake Angles**: Teeniz baktığınız yönün tersine bakar.
  - **Aimbot Troll Aim**: Her zaman en yakın oyuncuya nişan alır.

### **Other**
- **Change Name on Finish**: Bitiş çizgisini geçmeden hemen öncesinde isminizi otomatik olarak değiştirir.
- **Auto Team**: Seçilen takıma otomatik olarak katılır ve onu kilitler.
- **Anti AFK**: AFK olmayı önler.
- **Kill on Freeze**: Dondurulduğunuzda teenizi otomatik olarak öldürür.
- **Fast Input**: Girişinizi 1 tick daha hızlı (20ms) hissettirir, ancak bu yalnızca görsel bir etkidir.
- **Ignore Replay Warnings**: TAS tekrarlarıyla ilgili uyarı mesajlarını bastırır.
- **Hide Chat Bubble**: Sohbet balonunu gizler, böylece diğer oyuncular ne zaman yazdığınızı bilmez.
- **Auto Verify**: Beyaz liste korumalı sunucularda sizi otomatik olarak doğrular `ger10.ddnet.tw` gibi.
- **Send Occasional Ads**: Sohbette ara sıra reklamlar gönderir.

### **Troll**
- **Emote Spam**: Rastgele ifadeleri olabildiğince hızlı atar.
- **Killsay/Deathsays**: Öldürmeler veya ölümler üzerine önceden yazılmış mesajı gönderir.
- **Fancy Chat Font**: Benzersiz bir görünüm için sohbet yazı tipinizi değiştirir.
- **Mass Mention Spam**: Birden fazla oyuncudan tekrar tekrar bahseder.
- **Chat Repeater**: Başka bir oyuncunun sohbet mesajını otomatik olarak büyük ve küçük harflerle tekrarlar (örnek olarak, "MeSsAgE").

### **ID Stealer**
- **Enable**: ID Stealer özelliğini etkinleştirerek başka bir oyuncunun bilgilerini kopyalamanızı sağlar.
- **Closest Player**: Etkinleştirilmişse, bilgilerini kopyalamak için en yakın oyuncuyu hedefler. Devre dışı bırakılırsa, sunucuda rastgele bir oyuncu seçer.
- **Steal Name**: Hedeflenen oyuncunun adını kopyalar.
- **Steal Clan**: Hedeflenen oyuncunun klanını kopyalar.
- **Steal Skin**: Hedeflenen oyuncunun teesini kopyalar.
- **Steal Flag**: Hedeflenen oyuncunun bayrağını kopyalar.
- **Steal Eye Emote**: Hedeflenen oyuncunun ifadesi ifadesini kopyalar.
- **Stealer Speed**: Özelliğin çalınan detaylarını ne sıklıkta güncelleyeceğine ilişkin aralığı (saniye cinsinden) ayarlar.

### **Silent Walk**
- **Enable**: Hareketlerinizin diğer oyuncular tarafından daha az fark edilmesini sağlamak için belirli göstergeleri gizleyen Silent Walk özelliğini etkinleştirir.
- **Direction**: Hareket yönünüzü gösteren okları gizler.
- **Jump**: Zıplama okunu gizleyerek başkalarının ne zaman zıpladığınızı görmesini zorlaştırır.
- **Hook**: Hedefinize görünmez bir kanca gönderir. Kanca uzaklığının sınırlı olduğunu unutmayın.
- **Hook Closest**: En yakın oyuncuya görünmez bir kanca atar. Kanca uzaklığının sınırlı olduğunu unutmayın.

---

## **Configuration**

Çoğu kullanım durumu için aşağıdaki özellikleri etkinleştirmek faydalı olacaktır:
- **Auto Fire**: Silahınızı otomatik olarak ateşleyerek nişan almaya ve harekete odaklanmanızı kolaylaştırır.
- **Avoid Freeze**: Özellikle gores haritaları oynarken kullanışlı olan bu özellik, buzlardan kaçınmanıza yardımcı olur.
- **Quick Stop**: Block haritaları için harika olan bu özellik, hızlı ve hassas bir şekilde durmanıza yardımcı olur.
- **Auto Jump Save**: Donmayı önlemek için duruma bağlı bir özellik; gerektiğinde etkinleştirin.
- **Mod Detector**: Yetkililer tarafından izlenmekten veya yasaklanmaktan endişeleniyorsanız bunu kullanın.
- **Fast Input**: Birçok kullanıcı bunun tepki süresini artırmak için oyunun kurallarını değiştirdiğini söylüyor, bu yüzden bir deneyin.
- **Auto Verify**: DDOS korumalı sunucular için doğrulamayı otomatikleştiren bir özellik. Kolaylık sağlamak için açık tutmaya değer.

Bu özellikleri oyun ihtiyaçlarınıza göre ayarlayın ve tarzınıza en uygun kombinasyonu bulmak için denemeler yapın.