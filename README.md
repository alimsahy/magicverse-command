# Magicverse Standalone Inventory System

*__Hazirlayan__:* *Alimah YILDIRIM <alimsahy@gmail.com>*

# Komutlar
*Sistem içerisinde hazır bulunan önceden tanımlanmış yönetim komutları. 
Varsayılan Prefix: !*

---

## itemekle [item ismi] [item kısa isim]
*Sunucuya yeni bir item ekler.*

| Parametre      | Aldigi Deger    | Aciklama                                                                                  |
|----------------|-----------------|-------------------------------------------------------------------------------------------|
| item ismi      | String karakter | Eklenecek itemin tam ismi                                                                 |
| item kisa isim | String karakter | Daha sonra itemin ozelliklerini degistirmek icin veya item alirken kullanilacak kisa isim |

---

## itemset [alan] [item kisa isim] [deger]
*Mevcut itemin istenilen bir ozelligini gunceller. Boolean veri dondurur (True/False)*

| Parametre      | Aldigi Deger      | Aciklama                             |
|----------------|-------------------|--------------------------------------|
| alan           | String karakter   | Itemin degistirilecek ozelligi       |
| item kisa isim | String karakter   | Eklenen itemin kisa ismi             |
| deger          | Herhangi bir veri | Degistirilecek ozelligin yeni degeri |


*Item ozellik alanlari*
| Alan               | Aciklama                                                                          | Deger kismina girebilecek veri | Varsayilan Degerler |
|--------------------|-----------------------------------------------------------------------------------|--------------------------------|---------------------|
| aciklama           | Itemin mevcut aciklamasini degistirir                                             | Herhangi bir veri              | NULL                |
| ikon               | Itemin mevcut ikonunu gunceller                                                   | Discord emoji (:emoji:)        | NULL                |
| satis-fiyat        | Kullanicinin itemi alirken odemesi gereken ucreti gunceller                       | Sayi                           | 0                   |
| alis-fiyat         | Kullanicinin itemi iade ederken alacagi iade bedeli                               | Sayi                           | 0                   |
| tip                | Itemin kategorisini degistirir                                                    | Silah, Materyal veya Esya      | Esya                |
| yukseltilebilir    | Itemin yukseltilebilir ozelligi acar yada kapatir                                 | Evet yada Hayir                | Hayir               |
| yukseltilen-item   | Item yukseltildikten sonra hangi iteme donusecegi                                 | Item kisa ismi veya item id'si | 0                   |
| yukseltme-level    | Itemi yukseltmek icin gerekli olan seviye (ksks, sihirli ulasim vb)               | Sayi                           | 0                   |
| yukseltme-fiyat    | Itemi yukseltmek icin gerekli olan para miktari                                   | Sayi                           | 0                   |
| min-drop           | Kullanicilar RP yaparken bu itemden minimum kac tane dusurebileceklerini belirler | Sayi                           | 0                   |
| max-drop           | Kullanicilar RP yaparken bu itemden maximum kac adet dusurebileceklerini belirler | Sayi                           | 0                   |
| efsun              | Itemin efsun destegini aktif eder.                                                | Evet yada Hayir                | Hayir               |
| min-efsun          | Iteme minimum kac adet efsun gelebilecegini belirler                              | Sayi                           | 0                   |
| max-efsun          | Iteme maximum kac adet efsun gelebilecegini belirler                              | Sayi                           | 0                   |

---
