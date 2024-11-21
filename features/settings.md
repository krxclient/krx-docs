---
icon: gear
---

# Settings

KRX'teki **Settings** sekmesi, oyun deneyiminizi geliştirmek için kısayol tuşlarını yapılandırmanıza ve belirli özelliklere ince ayar yapmanıza olanak tanır.
---

## **Ekran Görüntüsü**
![Settings Menu](https://raw.githubusercontent.com/Krixx1337/krxclient-docs/refs/heads/main/images/settings-menu.png)

---

## **Hotkeys**
- **Aimbot**: Aimbot'u açar/kapatır.
- **Aimbot Auto Hook**: Aimbot etkinleştirildiğinde hedefi otomatik olarak kancalamayı açar/kapatır.
- **Aimbot Auto Shoot**: Aimbot etkinleştirildiğinde hedefe otomatik olarak çekiç vurmayı açar/kapatır.
- **Balance Bot**: Teelerde dengeyi korumak için denge botunu açar/kapatır.  
- **Emote Spam**: Sürekli ifade spamlamayı açar/kapatır.  
- **Hook Spam**: Hızlı kanca spamlamayı açar/kapatır.    
- **Super DynCam**: Dinamik kamera için sınırsız yakınlaştırmayı açar/kapatır.    
- **Pixel Walk**: Yön tuşlarını kullanırken hassas, piksel piksel hareket etmeyi açar/kapatır.  
- **Hook Nearest Collision**: En yakın duvara otomatik olarak kanca atmayı açar/kapatır. 
- **Quick Stop**: Mümkün olduğunca hızlı durmak için herhangi bir yön tuşunu basılı tutmadığınızda durursunuz bu özelliği açar/kapatır.
- **Hook Ride (riskli)**: Hook ride botu açar/kapatır.  
- **Record Replay**: Oyuncunun hareketlerini kayıt etmeyi açar/kapatır.  
- **Load Replay**: Oyuncunun hareketlerini oynatmayı açar/kapatır.  
- **Avoid Freeze**: Buzlardan kaçınmaya yardımcı olmak için botu açar/kapatır.  
- **Auto Edge**: Botun donma, ölüm veya ışınlanma bloklarında yakınındaki kenarlara otomatik olarak inmesini sağlamayı açar/kapatır. ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)  
- **Laser Unfreeze Bot**: Lazer kullanarak sizi otomatik olarak kurtarması için bir botu açar/kapatır. ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)  
- **Avoid Auto Drag**: Bu özellik aktif olduğunda donmadan en yakın tee'yi otomatik olarak taşımayı açar/kapatır. ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)  
- **Avoid Track Points**: Blatant Gores Bot için gelişmiş nokta takibini açar/kapatır. Detaylar için [Blatant Gores Bot](blatant.md)'a bakın. ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)  

---

## **Settings**
- **Teleport Prediction**: TAS veya Gores Bot için ışınlanma tahminini etkinleştirir, aksi takdirde ışınlanmalar donma ile değiştirilir. ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square) 
- **Advanced Settings**: Maksimum avantaj için tüm KRX botlarına ince ayar yapmak için gelişmiş tahmin ayarlarının kilidini açar: ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)
   - **Death Tile Prediction**: TAS ve Gores Bot dahil olmak üzere botlar için ölüm bloklarını tahmin eder. Aksi takdirde, ölüm blokları yok sayılır.  
   - **Move Restrictions Prediction**: Hava durdurucuları tahmin eder. Bunu devre dışı bırakmak bot performansını önemli ölçüde artırabilir.  
   - **Player Loop**: Tee çarpışmalarını tahmin eder. Bunu devre dışı bırakmak yalnızca çarpışma işlemeyi kaldırır ve bot performansını önemli ölçüde artırabilir. 
   - **Prediction Margin**: Tahmin margini ayarlar. Daha yüksek değerler gecikme artışlarından daha az etkilenmenizi sağlar ancak diğerlerinin daha gecikmeli görünmesine neden olabilir.
- **Balance Bot Offset**: Denge botunun dengeyi korumak için ne kadar agresif tepki vereceğini yapılandırır. Daha yüksek değerler hareket düzeltmelerini azaltır.  
- **Hook Nearest FOV**:  **Hook Nearest Collision** özelliği için fovu ayarlar.  

---

## **Configuration**

1. KRX'teki **Settings** sekmesini açın.  
2. Tercihlerinize göre özelliklere özel kısayol tuşları atayın.
3. Ayarları oyun ihtiyaçlarınıza uyacak şekilde yapın. Aşağıda bazı **önerilen yapılandırmalar** bulunmaktadır:  
   - **Teleport Prediction**: TAS kullanılmadığı sürece devre dışı bırakılması önerilir. Gores Bot'u kullanırken etkinleştirmeyin. ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)  
   - **Advanced Settings**: Nasıl kullanıldığını bilmiyorsanız devre dışı bırakmanız önerilir. ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)  
      - **Death Tile Prediction**: Botları yavaşlattığı için devre dışı bırakılması önerilir, ancak TAS için yararlıdır. 
      - **Move Restrictions Prediction**: Normal oyun için etkinleştirilmesi önerilir. Botlarda önemli performans artışları için devre dışı bırakın.  
      - **Player Loop**: Normal oyun için etkinleştirilmesi önerilir. Botlarda önemli performans artışları için devre dışı bırakın.  
      - **Prediction Margin**: Ping değerinize göre bir değer seçin (örneğin, 50 ms ping için ~50 olarak ayarlayın). Bot sorunlarını önlemek için daha yüksek değerler (>20) ayarlanması önerilir.
   - **Balance Bot Offset**: Önerilen Değer: ~2.  
   - **Hook Nearest FOV**: Düşük CPU'larda lagı azaltmak için daha düşük FOV ayarlanması önerilir (örnek olarak , 30) .  